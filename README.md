# Karamazov RAG

*An exploration of Retrieval-Augmented Generation: a small, fully traceable RAG system over Dostoevsky's* The Brothers Karamazov *and five scholarly papers about it, and a study of where and why it fails.*

Ask a question about the novel or the papers, and the system answers **only from retrieved passages**, citing the exact chapter (`Part II › Book V › Chapter V. The Grand Inquisitor`) or PDF page (`Namli (2022) — PDF p. 8`) for each claim. Everything runs in one Google Colab notebook on a free T4 GPU with open models.

The exploration focuses on **evaluation and failure analysis**: when an answer is wrong, did **retrieval** fail (the evidence never reached the model) or did **generation** fail (the evidence was there but misused)?

---

## Pipeline

```
OFFLINE (once)
 EPUB novel ──► structural parse (Part › Book › Chapter) ─┐
 5 PDF papers ─► per-page text, headers/footers & refs cut ┴─► chunks (≤400 tok, 60 overlap) ─► bge-base embeddings ─► FAISS
                                                                                             └─────────────────────► BM25
ONLINE (per question)
 question ─► retrieve top-5 (dense | BM25 | hybrid RRF) ─► prompt with [S1]…[S5] + locations
          ─► Qwen3-4B-Instruct (greedy) ─► answer with [S#] citations
          ─► citation check (valid / invalid / abstained) ─► runs.jsonl + Langfuse trace
```

![Langfuse trace of one query in dense mode: retrieval takes 0.01 s and generation 12 s; the first retrieved chunk is Namli (2022), PDF p. 17, with its rank, score and text preview. BM25 fields are null because this run used dense retrieval only.](docs/langfuse_trace.png)

---

## Tools and models

| Component | Choice | Why |
|---|---|---|
| LLM | `Qwen/Qwen3-4B-Instruct-2507` (fp16) | Fits a free T4 (~8 GB); good instruction following; no hidden "thinking" output |
| Embeddings | `BAAI/bge-base-en-v1.5` | Solid English retrieval model; 512-token limit fits 400-token chunks |
| Vector search | FAISS `IndexFlatIP` (exact cosine) | 1,735 chunks → exact search in milliseconds, no server |
| Keyword search | `rank_bm25` (BM25Okapi) | Exact names and spellings |
| Parsing | `ebooklib` + BeautifulSoup (EPUB), PyMuPDF (PDF) | Structure-aware EPUB; page-level PDF text |
| Observability | Langfuse (SDK v5) + local JSONL | One trace per question: retrieval → prompt → generation |
| Runtime | Google Colab, T4 GPU, `transformers 5.22.1` | Free GPU, no local setup |

---

## Approach

- **Ingestion:** the EPUB's semantic markup is read directly, so every chunk has an exact Part › Book › Chapter label. PDFs are read page by page; repeating headers and footers, page numbers and reference lists are removed, and hyphenated words are re-joined.
- **Chunking:** paragraphs are packed into chunks of ≤ 400 tokens with 60 tokens of overlap. Chunks never cross a chapter or a page, so each has a single citable location.
- **Retrieval:** three modes. **Dense** (embeddings + FAISS), **BM25** (keywords), and **hybrid**, which merges both rankings with Reciprocal Rank Fusion (score = Σ 1/(60 + rank)). Top 5 passages per question.
- **Generation:** a prompt that allows only the numbered sources, requires `[S#]` citations, defines an explicit "not enough information" answer, and caps context at 3,000 tokens. Greedy decoding keeps runs reproducible.
- **Attribution check:** every `[S#]` is mapped back to the chunk that was actually in the prompt; invalid citations, uncited answers and abstentions are flagged automatically.
- **Evaluation:** 18 questions (single-passage, cross-passage, paper, cross-document, a spelling-variant probe, and 2 unanswerable). Gold labels mark *where* the evidence is (chapter or paper). Metrics: Hit@5, Recall@5, MRR, abstention and gold-citation rate, plus a closed-book baseline (same LLM, no retrieval).

---

## Configuration

All settings live in one `Config` dataclass and can be overridden with environment variables (see `.env.example`):

| Variable | Default | Meaning |
|---|---|---|
| `RAG_LLM_MODEL` | `Qwen/Qwen3-4B-Instruct-2507` | any Hugging Face chat model |
| `RAG_EMBED_MODEL` | `BAAI/bge-base-en-v1.5` | embedding model |
| `RAG_CHUNK_SIZE` / `RAG_CHUNK_OVERLAP` | `400` / `60` | tokens |
| `RAG_RETRIEVAL_MODE` | `dense` | `dense`, `bm25` or `hybrid` (hybrid recommended) |
| `RAG_TOP_K` | `5` | passages per question |
| `RAG_MAX_CONTEXT_TOKENS` / `RAG_MAX_NEW_TOKENS` | `3000` / `400` | context budget / answer length |
| `RAG_USE_LANGFUSE` | `auto` | tracing on when Langfuse keys are present |

---

## Results

**Retrieval** (16 answerable questions, k = 5, no LLM involved):

| Mode | Hit@5 | Recall@5 | MRR |
|---|---|---|---|
| Dense | 0.812 | 0.750 | 0.762 |
| BM25 | 0.875 | 0.812 | 0.771 |
| Hybrid | 0.875 | 0.812 | 0.674 |

**End to end** (18 questions):

| | Dense | Hybrid |
|---|---|---|
| Answers citing the correct chapter/paper (of 16) | 11 | **12** |
| Unnecessary abstentions | 4 | **3** |
| Correct abstentions on unanswerable questions | 2 / 2 | 2 / 2 |
| Invalid citations | 0 | 0 |
| Median time per question | 10.2 s | 9.7 s |

**Key findings:**
- **Hybrid is the best default:** more evidence found and more grounded answers than dense, at no extra latency. But no mode wins everywhere: BM25 wins on exact spellings ("Zossima"), dense on paraphrase, hybrid when two sources are needed. RRF's lower MRR shows it can outvote a hit that only one retriever ranks first.
- **Retrieval vs generation:** some failures are retrieval misses (spelling variants; a paper's summary outranking the novel's chapter). Others are generation failures: in q06 the right passage was retrieved at rank 5 and the model still answered "not enough information".
- **Faithful ≠ correct:** asked for Mitya's sentence, the system cited a paper saying "ten years". The citation was accurate, but the novel says **twenty**.
- **The model barely knows the novel on its own:** without retrieval it answered "I don't know" to 7 of 16 questions and got most others wrong, so correct specifics come from retrieval.
- **Generation dominates latency:** retrieval takes about 17 ms, generation about 10 s (99%+ of the time).

With 16 questions, one question is a 0.06 difference, so these are indications rather than statistically conclusive results. Per-question passages, answers and sources are in `outputs/eval_report_{dense,hybrid}.md`.

---

## Documents

| Document | File name | License | Source |
|---|---|---|---|
| F. Dostoevsky, *The Brothers Karamazov*, trans. C. Garnett (1912), Standard Ebooks edition | `fyodor-dostoevsky_the-brothers-karamazov_constance-garnett.epub` | Public domain (US); edition CC0 | [standardebooks.org/ebooks/fyodor-dostoevsky/the-brothers-karamazov/constance-garnett](https://standardebooks.org/ebooks/fyodor-dostoevsky/the-brothers-karamazov/constance-garnett) |
| Osińska & Szejko (2021), *The Mystery of the Crime in Skotoprigonyevsk* | `osinska2021.pdf` | CC BY 4.0 | [preprints.org/manuscript/202111.0493](https://www.preprints.org/manuscript/202111.0493) |
| Roberts (2018), *Love, attention and teaching: Dostoevsky's The Brothers Karamazov* | `love_teaching2018.pdf` | CC BY | [doi.org/10.1080/23265507.2017.1404434](https://doi.org/10.1080/23265507.2017.1404434) |
| Admirand (2021), *Theist–Atheist Encounters in Les Misérables, The Brothers Karamazov, and The Plague* | `admirand2021.pdf` | CC BY | [mdpi.com/2077-1444/12/1/12](https://www.mdpi.com/2077-1444/12/1/12) |
| Namli (2022), *The Brothers Karamazov and the theology of suffering* | `namli2022.pdf` | CC BY 4.0 | [doi.org/10.1007/s11212-021-09454-x](https://doi.org/10.1007/s11212-021-09454-x) |
| Gabor (2024), *The Problem of Evil and Fr. Zosima's Responsibility Before All* | `gabor2024.pdf` | CC BY-NC-ND 4.0 | [doi.org/10.2478/ress-2024-0009](https://doi.org/10.2478/ress-2024-0009) |

About 394k words, 1,735 chunks in total. The files are **not included** in this repository; download them from the sources above.

---

## Running it

1. Download the six documents from the **Source** links above and put them in `MyDrive/karamazov_rag_data/`, using the file names in the table (the EPUB name can be anything).
2. Open `karamazov_rag.ipynb` in Google Colab and select a **T4 GPU** runtime.
3. *(Optional)* Add `LANGFUSE_PUBLIC_KEY`, `LANGFUSE_SECRET_KEY`, `LANGFUSE_BASE_URL` as Colab Secrets for tracing.
4. **Run all** and allow Drive access. In the interactive cell, type a question, `:mode hybrid` to switch retrieval, or Enter on an empty line to stop.

Needs a GPU with ~10 GB VRAM (free Colab T4 is enough). First run takes about 10 min (downloads and embedding), then about 10 s per question.

---

## Repository

```
├── karamazov_rag.ipynb      # the whole pipeline, with saved outputs
├── requirements.txt
├── .env.example             # configuration template (no credentials)
├── docs/
│   └── langfuse_trace.png
└── outputs/
    ├── retrieval_comparison.csv          # dense vs BM25 vs hybrid
    ├── eval_report_{dense,hybrid}.md     # every question: passages, answer, sources
    ├── eval_summary_{dense,hybrid}.csv
    ├── eval_results_{dense,hybrid}.jsonl
    ├── closed_book_baseline.md           # same LLM, no retrieval
    └── runs.jsonl                        # every query with its full trace record
```
