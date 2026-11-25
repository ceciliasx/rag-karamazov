# Evaluation report
- LLM: `Qwen/Qwen3-4B-Instruct-2507`  
- Embeddings: `BAAI/bge-base-en-v1.5`  
- Retrieval: `hybrid`, top_k=5, chunk=400 tok, overlap=60  
- Generated: 2026-11-23 06:49

## q01 (single) — In Ivan's poem, what three forces does the Grand Inquisitor say can hold people captive forever?
Retrieval: hit=1 recall=1.0 MRR=0.333 | abstained=False | cites gold=False | invalid citations=[]

**RAG answer:**
The Grand Inquisitor says that the three forces capable of holding people captive forever are "miracle, mystery and authority" [S4]. These correspond to the three temptations Christ faced in the wilderness: turning stones into bread, leaping from the pinnacle of the temple, and ruling over all kingdoms [S4]. The Inquisitor argues that by rejecting these temptations, Christ gave humanity freedom, which is too burdensome; thus, the Church stepped in to provide these three forces to ensure human happiness and obedience [S4]. This view is echoed in the text where the Inquisitor claims that these forces are what people truly desire, not freedom [S4].

**Cited:** [S4] Love, attention and teaching (2018) — PDF p. 6 (`love_teaching2018-0014`)

**Closed-book answer (no retrieval):**
(not run)

<details><summary>Retrieved passages</summary>

- **S1** score=0.032 `love_teaching2018-0013` — Love, attention and teaching (2018) — PDF p. 5  
  Ivan raises further questions in his prose poem of the Grand Inquisitor. Set in sixteenth century Seville, his poem describes the reappearance of Christ, who walks among people on the streets, radiating love and compassion (Sandoz, 1964, pp. 359–360). He performs a miracle, raising a young girl from the dead, and is worshipped by those who see him. His

- **S2** score=0.0318 `love_teaching2018-0015` — Love, attention and teaching (2018) — PDF p. 6  
  Aware that God does not exist, they have created Christianity as an ‘elaborate myth’ with a view to controlling and organising ‘rebellious imaginations’ (p. xv). Their goal, however, has been a noble one: by manipulating people in this manner, they have restricted their freedom but enhanced their happiness. The Church forefathers recognised that we can have freedom or happiness, but not both. The Church has provided what human beings seek. They want others to serve as their consciences; they want to ‘bow down’ to others; and they want to be formed into ‘a common, concordant and [...]

- **S3** score=0.0303 `karamazov-0486` — The Brothers Karamazov (Garnett) — Part II › Book V. Pro and Contra › Chapter V. The Grand Inquisitor  
  But didst Thou not know that he would at last reject even Thy image and Thy truth, if he is weighed down with the fearful burden of free choice? They will cry aloud at last that the truth is not in Thee, for they could not have been left in greater confusion and suffering than Thou hast caused, laying upon them so many cares and unanswerable problems. “ ‘So that, in truth, Thou didst Thyself lay the foundation for the destruction of Thy kingdom, and no one is more to blame for it. Yet what was offered Thee? There are three powers, three powers alone, able to conquer and to hold captive [...]

- **S4** score=0.0301 `love_teaching2018-0014` — Love, attention and teaching (2018) — PDF p. 6  
  actions come to the attention of the Grand Inquisitor, a ninety year old Roman Catholic Cardinal, who has sanctioned the burning of dozens of heretics just prior to Christ’s arrival. The Grand Inquisitor summons Christ to his cell and admonishes the latter for disrupting order in the town. Motivated by his love for humankind, the Grand Inquisitor advises Christ that he too will have to be put to death. The people may praise him today, the Grand Inquisitor says to Christ, but tomorrow they could just as easily turn on him and call for his blood. Through Christ, people are granted moral [...]

- **S5** score=0.0299 `karamazov-0500` — The Brothers Karamazov (Garnett) — Part II › Book V. Pro and Contra › Chapter V. The Grand Inquisitor  
  “I meant to end it like this. When the Inquisitor ceased speaking he waited some time for his Prisoner to answer him. His silence weighed down upon him. He saw that the Prisoner had listened intently all the time, looking gently in his face and evidently not wishing to reply. The old man longed for Him to say something, however bitter and terrible. But He suddenly approached the old man in silence and softly kissed him on his bloodless aged lips. That was all His answer. The old man shuddered. His lips moved. He went to the door, opened it, and said to Him: ‘Go, and come no more … come [...]

</details>

## q02 (single) — What story about a serf boy and a general's hounds does Ivan tell Alyosha, and why does he tell it?
Retrieval: hit=1 recall=1.0 MRR=0.5 | abstained=False | cites gold=True | invalid citations=[]

**RAG answer:**
Ivan tells Alyosha the story of a serf-boy, eight years old, who throws a stone that hurts the paw of a general’s favorite hound. The general, enraged, strips the boy naked, orders him to run, and then sets his pack of hounds on him, tearing him to pieces before his mother’s eyes. The story is set during the dark days of serfdom and is told to illustrate the moral absurdity of unchecked power and cruelty, challenging theistic faith by presenting a horrific act that cannot be justified or ignored [S1][S2][S3][S4]. Ivan tells it to provoke Alyosha’s moral reflection and to demonstrate that the world is built on such absurdities, even if they are morally repugnant [S3].

**Cited:** [S1] Admirand (2021) — PDF p. 13 (`admirand2021-0044`); [S2] The Brothers Karamazov (Garnett) — Part II › Book V. Pro and Contra › Chapter IV. Rebellion (`karamazov-0462`); [S3] The Brothers Karamazov (Garnett) — Part II › Book V. Pro and Contra › Chapter IV. Rebellion (`karamazov-0463`); [S4] Gabor (2024) — PDF p. 6 (`gabor2024-0013`)

**Closed-book answer (no retrieval):**
(not run)

<details><summary>Retrieved passages</summary>

- **S1** score=0.0325 `admirand2021-0044` — Admirand (2021) — PDF p. 13  
  Eleanora” who is born and dies in the camps, despite the desperate pleas and prayers of her mother to God. Ivan, too, has cut to the heart of the impossible challenge brought to theists, impossible to justify or to ignore if theistic faith can somehow be maintained.84 Knowing he has struck a chord, Ivan apologizes for upsetting Alyosha, but his younger brother tells him to proceed. So, Ivan presents the story of a “house-serf” who accidentally hurt the favourite hound of his master, a general from an aristocratic family. The boy had thrown a stone which hit the dog’s paw. Because of the [...]

- **S2** score=0.0323 `karamazov-0462` — The Brothers Karamazov (Garnett) — Part II › Book V. Pro and Contra › Chapter IV. Rebellion  
  “Never mind. I want to suffer too,” muttered Alyosha. “One picture, only one more, because it’s so curious, so characteristic, and I have only just read it in some collection of Russian antiquities. I’ve forgotten the name. I must look it up. It was in the darkest days of serfdom at the beginning of the century, and long live the Liberator of the People! There was in those days a general of aristocratic connections, the owner of great estates, one of those men—somewhat exceptional, I believe, even then—who, retiring from the service into a life of leisure, are convinced that they’ve [...]

- **S3** score=0.0315 `karamazov-0463` — The Brothers Karamazov (Garnett) — Part II › Book V. Pro and Contra › Chapter IV. Rebellion  
  The servants are summoned for their edification, and in front of them all stands the mother of the child. The child is brought from the lockup. It’s a gloomy, cold, foggy autumn day, a capital day for hunting. The general orders the child to be undressed; the child is stripped naked. He shivers, numb with terror, not daring to cry. … ‘Make him run,’ commands the general. ‘Run! run!’ shout the dog-boys. The boy runs. … ‘At him!’ yells the general, and he sets the whole pack of hounds on the child. The hounds catch him, and tear him to pieces before his mother’s eyes! … I believe the [...]

- **S4** score=0.0302 `gabor2024-0013` — Gabor (2024) — PDF p. 6  
  Ivan then strengthens this claim with the story in which the general murders a child before the eyes of the child’s mother. The boy had thrown a stone which made the general’s dog limp. After locking the boy overnight, the general acts in unthinkable ways: It was a dark, cold, foggy autumn day, splendid for hunting. The General ordered that the child be undressed, and he stood there stark naked, shivering and petrified with fear, not daring to make one sound… “Make him run!” ordered the General. “Run, run!” the huntsmen shouted at him, and the boy ran… “After him!” roared the General, [...]

- **S5** score=0.0296 `karamazov-1105` — The Brothers Karamazov (Garnett) — Part IV › Book XI. Ivan › Chapter I. At Grushenka’s  
  “Yes, there’s a fearful accumulation of evidence,” Alyosha observed grimly. “And Grigory—Grigory Vassilyevitch—sticks to his story that the door was open, persists that he saw it—there’s no shaking him. I went and talked to him myself. He’s rude about it, too.” “Yes, that’s perhaps the strongest evidence against him,” said Alyosha. “And as for Mitya’s being mad, he certainly seems like it now,” Grushenka began with a peculiarly anxious and mysterious air. “Do you know, Alyosha, I’ve been wanting to talk to you about it for a long time. I go to him every day and simply wonder at him. Tell [...]

</details>

## q03 (single) — What happened to the elder's body after his death, and how did people react?
Retrieval: hit=1 recall=1.0 MRR=0.25 | abstained=False | cites gold=True | invalid citations=[]

**RAG answer:**
After Father Zossima’s death, his body was laid in a coffin and brought into the front room. The monks anticipated decay, and by midday, signs of decomposition became evident—first noticed in silence, then openly reported by three o’clock. The news spread quickly through the hermitage, monastery, and town, causing astonishment. Unbelievers rejoiced, while some believers also rejoiced, as the deceased elder had taught that “men love the downfall and disgrace of the righteous.” The reaction was mixed: some were mortified by the smell, others delighted, and there was deep-seated jealousy and hostility toward Zossima’s saintliness, which fueled the incident [S4][S5]. The smell of decomposition was seen as absurd by some, who expected something more holy [S5].

**Cited:** [S4] The Brothers Karamazov (Garnett) — Part III › Book VII. Alyosha › Chapter I. The Breath of Corruption (`karamazov-0633`); [S5] The Brothers Karamazov (Garnett) — Part III › Book VII. Alyosha › Chapter I. The Breath of Corruption (`karamazov-0630`)

**Closed-book answer (no retrieval):**
(not run)

<details><summary>Retrieved passages</summary>

- **S1** score=0.0325 `karamazov-0042` — The Brothers Karamazov (Garnett) — Part I › Book I. The History of a Family › Chapter V. Elders  
  The story is told, for instance, that in the early days of Christianity one such novice, failing to fulfill some command laid upon him by his elder, left his monastery in Syria and went to Egypt. There, after great exploits, he was found worthy at last to suffer torture and a martyr’s death for the faith. When the Church, regarding him as a saint, was burying him, suddenly, at the deacon’s exhortation, “Depart all ye unbaptized,” the coffin containing the martyr’s body left its place and was cast forth from the church, and this took place three times. And only at last they learnt that [...]

- **S2** score=0.0315 `karamazov-0624` — The Brothers Karamazov (Garnett) — Part II › Book VI. The Russian Monk › Chapter III. Conversations and Exhortations of Father Zossima  
  The elder’s death came in the end quite unexpectedly. For although those who were gathered about him that last evening realized that his death was approaching, yet it was difficult to imagine that it would come so suddenly. On the contrary, his friends, as I observed already, seeing him that night apparently so cheerful and talkative, were convinced that there was at least a temporary change for the better in his condition. Even five minutes before his death, they said afterwards wonderingly, it was impossible to foresee it. He seemed suddenly to feel an acute pain in his chest, he [...]

- **S3** score=0.0301 `karamazov-0306` — The Brothers Karamazov (Garnett) — Part II › Book IV. Lacerations › Chapter I. Father Ferapont  
  When Alyosha happened for a moment to leave the cell, he was struck by the general excitement and suspense in the monks who were crowding about it. This anticipation showed itself in some by anxiety, in others by devout solemnity. All were expecting that some marvel would happen immediately after the elder’s death. Their suspense was, from one point of view, almost frivolous, but even the most austere of the monks were affected by it. Father Païssy’s face looked the gravest of all.

- **S4** score=0.0301 `karamazov-0633` — The Brothers Karamazov (Garnett) — Part III › Book VII. Alyosha › Chapter I. The Breath of Corruption  
  Yet, in spite of these edifying memories, it would be difficult to explain the frivolity, absurdity and malice that were manifested beside the coffin of Father Zossima. It is my private opinion that several different causes were simultaneously at work, one of which was the deeply-rooted hostility to the institution of elders as a pernicious innovation, an antipathy hidden deep in the hearts of many of the monks. Even more powerful was jealousy of the dead man’s saintliness, so firmly established during his lifetime that it was almost a forbidden thing to question it. For though the late [...]

- **S5** score=0.0277 `karamazov-0630` — The Brothers Karamazov (Garnett) — Part III › Book VII. Alyosha › Chapter I. The Breath of Corruption  
  And so, to return to our story. When before dawn they laid Father Zossima’s body in the coffin and brought it into the front room, the question of opening the windows was raised among those who were around the coffin. But this suggestion made casually by someone was unanswered and almost unnoticed. Some of those present may perhaps have inwardly noticed it, only to reflect that the anticipation of decay and corruption from the body of such a saint was an actual absurdity, calling for compassion (if not a smile) for the lack of faith and the frivolity it implied. For they expected [...]

</details>

## q04 (single) — What vision does Alyosha have while the Gospel is read over the elder's coffin, and how does it change him?
Retrieval: hit=1 recall=1.0 MRR=1.0 | abstained=True | cites gold=True | invalid citations=[]

**RAG answer:**
Alyosha does not have a vision while the Gospel is read over the elder's coffin. Instead, he experiences a profound emotional and spiritual awakening. As the Gospel is read, something "glowed in Alyosha’s heart," filling it with rapture and causing tears of joy to rise [S2]. He falls asleep on his knees, then wakes up and moves toward the coffin, gazing at it with deep emotion. This moment transforms him: his soul is "overflowing with rapture," and he longs for freedom and openness, seeing the night sky and the stars as a reflection of divine mystery [S2]. The experience deepens his spiritual connection, though no explicit vision is described. The provided sources do not contain enough information to describe a vision in the literal sense.

**Cited:** [S2] The Brothers Karamazov (Garnett) — Part III › Book VII. Alyosha › Chapter IV. Cana of Galilee (`karamazov-0697`)

**Closed-book answer (no retrieval):**
(not run)

<details><summary>Retrieved passages</summary>

- **S1** score=0.0323 `karamazov-0691` — The Brothers Karamazov (Garnett) — Part III › Book VII. Alyosha › Chapter IV. Cana of Galilee  
  It was very late, according to the monastery ideas, when Alyosha returned to the hermitage; the doorkeeper let him in by a special entrance. It had struck nine o’clock—the hour of rest and repose after a day of such agitation for all. Alyosha timidly opened the door and went into the elder’s cell where his coffin was now standing. There was no one in the cell but Father Païssy, reading the Gospel in solitude over the coffin, and the young novice Porfiry, who, exhausted by the previous night’s conversation and the disturbing incidents of the day, was sleeping the deep sound sleep of youth [...]

- **S2** score=0.032 `karamazov-0697` — The Brothers Karamazov (Garnett) — Part III › Book VII. Alyosha › Chapter IV. Cana of Galilee  
  Something glowed in Alyosha’s heart, something filled it till it ached, tears of rapture rose from his soul. … He stretched out his hands, uttered a cry and waked up. Again the coffin, the open window, and the soft, solemn, distinct reading of the Gospel. But Alyosha did not listen to the reading. It was strange, he had fallen asleep on his knees, but now he was on his feet, and suddenly, as though thrown forward, with three firm rapid steps he went right up to the coffin. His shoulder brushed against Father Païssy without his noticing it. Father Païssy raised his eyes for an instant [...]

- **S3** score=0.0303 `karamazov-0644` — The Brothers Karamazov (Garnett) — Part III › Book VII. Alyosha › Chapter I. The Breath of Corruption  
  “This is the one who is a saint! This is the one who is a holy man!” some cried aloud, losing their fear. “This is he who should be an elder,” others added malignantly. “He wouldn’t be an elder … he would refuse … he wouldn’t serve a cursed innovation … he wouldn’t imitate their foolery,” other voices chimed in at once. And it is hard to say how far they might have gone, but at that moment the bell rang summoning them to service. All began crossing themselves at once. Father Ferapont, too, got up and crossing himself went back to his cell without looking round, still uttering [...]

- **S4** score=0.0301 `karamazov-0045` — The Brothers Karamazov (Garnett) — Part I › Book I. The History of a Family › Chapter V. Elders  
  Alyosha noticed that many, almost all, went in to the elder for the first time with apprehension and uneasiness, but came out with bright and happy faces. Alyosha was particularly struck by the fact that Father Zossima was not at all stern. On the contrary, he was always almost gay. The monks used to say that he was more drawn to those who were more sinful, and the greater the sinner the more he loved him. There were, no doubt, up to the end of his life, among the monks some who hated and envied him, but they were few in number and they were silent, though among them were some of great [...]

- **S5** score=0.0298 `karamazov-1509` — The Brothers Karamazov (Garnett) — Epilogue › Chapter III. Ilusha’s Funeral. The Speech at the Stone  
  “That’s a good thing,” said Alyosha, “we must often take some.” “Every day, every day!” said the captain quickly, seeming cheered at the thought. They reached the church at last and set the coffin in the middle of it. The boys surrounded it and remained reverently standing so, all through the service. It was an old and rather poor church; many of the icons were without settings; but such churches are the best for praying in. During the mass Snegiryov became somewhat calmer, though at times he had outbursts of the same unconscious and, as it were, incoherent anxiety. At one moment he went [...]

</details>

## q05 (alias) — What does Zosima say about love in action compared with love in dreams?
Retrieval: hit=0 recall=0.0 MRR=0.0 | abstained=False | cites gold=False | invalid citations=[]

**RAG answer:**
Zosima says that active love is very different from the love encountered in dreams. In dreams, love may be immediate, with instant recognition and reward. In contrast, active love requires hard work, persistence, and often shows no immediate returns; it is hidden from public view and not easily recognized. He emphasizes that active love is not for the faint-hearted and that it is tested by expressions of ingratitude, unlike the immediate satisfaction found in dreams [S1].

**Cited:** [S1] Love, attention and teaching (2018) — PDF p. 5 (`love_teaching2018-0011`)

**Closed-book answer (no retrieval):**
(not run)

<details><summary>Retrieved passages</summary>

- **S1** score=0.0325 `love_teaching2018-0011` — Love, attention and teaching (2018) — PDF p. 5  
  Madame Khokhlakov then goes on to indicate that although she has sometimes dreamed of leaving Liza in order to nurse the suffering, she has doubts about her ability to sustain such a mission (pp. 56–57). She fears that her commitment to active love would be tested and undermined by expressions of ingratitude. Father Zosima demonstrates sympathy for her position, recalling that he once heard similar sentiments being expressed by a doctor. The doctor had noted that he loved humankind, but that the stronger his love was in this direction, the less able he was to love people in particular [...]

- **S2** score=0.0312 `love_teaching2018-0016` — Love, attention and teaching (2018) — PDF p. 6  
  An answer to the Grand Inquisitor is provided by life and teachings of Father Zosima, as set out in Book 6 (‘The Russian Monk’). Alyosha assumes responsibility for recording the elderly monk’s thoughts, making them available after Zosima’s death. These writings constitute an indirect repudiation of the idea of everything being permitted and an affirmation of the principle of active love espoused by Zosima in his earlier interactions with Madame Khokhlakov and her daughter. We discover that a pivotal event in the life of Zosima was the death of his older brother, Markel, as a teenager. [...]

- **S3** score=0.0311 `gabor2024-0022` — Gabor (2024) — PDF p. 11  
  In Fr. Zosima’s case, he acknowledges that the love he receives comes from above. He has been embraced always, regardless of what he has done in his youth and regardless of what he does every day. While Dostoevsky built the character of Fr. Zosima on St. Ambrose of Optina, his name also reminds us of the story of Mary of Egypt, who after 47 years in the desert met another Zosima and told him her life story in great humility. Prior to her life in the desert, Mary had lived a dissolute existence. One day, she joined a group sailing toward Jerusalem. These people had the intention to [...]

- **S4** score=0.0305 `gabor2024-0010` — Gabor (2024) — PDF p. 5  
  In our context, Ivan’s description of the world denies Zosima’s, but Zosima’s does not contradict Ivan’s. Instead, it embraces it. The result is that the world of suffering is no longer denied; a heavenly life can take place in the middle of suffering, as long as you share it with someone else. The famous chapter “Rebellion” begins with Ivan’s statement about the impossibility of love. “I could never understand how one could love one’s neighbor. In my opinion, it’s precisely those who are near us that it is impossible to love, and one can only love those who are distant from us.”17 Then [...]

- **S5** score=0.0304 `love_teaching2018-0008` — Love, attention and teaching (2018) — PDF p. 4  
  Beyond reason? love in The Brothers Karamazov The importance of love as a theme in The Brothers Karamazov is evident from early on in the novel. In Book II, Father Zosima receives a number of visitors at the monastery. At the centre of one group is Fyodor Karamazov, who embarrasses himself and others with his buffoonery. Among the others who seek the elder’s advice, however, is Madame Khokhlakov, who has arrived with her daughter, Liza. Liza suffers from paralysis of the legs and is in a wheelchair. Prior to speaking with Father Zosima, Madame Khokhlakov observes an exchange with another [...]

</details>

## q06 (single) — Who was Smerdyakov's mother, and what happened to her?
Retrieval: hit=1 recall=1.0 MRR=0.2 | abstained=True | cites gold=True | invalid citations=[]

**RAG answer:**
The provided sources do not contain enough information to answer this. While [S5] mentions that Smerdyakov was named after his mother’s nickname and that he was a servant employed as cook, it does not identify his mother’s name or describe what happened to her. No other source provides details about her identity or fate.

**Cited:** [S5] The Brothers Karamazov (Garnett) — Part I › Book III. The Sensualists › Chapter II. Lizaveta (`karamazov-0182`)

**Closed-book answer (no retrieval):**
(not run)

<details><summary>Retrieved passages</summary>

- **S1** score=0.0325 `karamazov-1196` — The Brothers Karamazov (Garnett) — Part IV › Book XI. Ivan › Chapter VII. The Second Visit to Smerdyakov  
  By that time Smerdyakov had been discharged from the hospital. Ivan knew his new lodging, the dilapidated little wooden house, divided in two by a passage on one side of which lived Marya Kondratyevna and her mother, and on the other, Smerdyakov. No one knew on what terms he lived with them, whether as a friend or as a lodger. It was supposed afterwards that he had come to stay with them as Marya Kondratyevna’s betrothed, and was living there for a time without paying for board or lodging. Both mother and daughter had the greatest respect for him and looked upon him as greatly superior [...]

- **S2** score=0.031 `osinska2021-0006` — Osińska & Szejko (2021) — PDF p. 4  
  dialoging subject or a rhetorical object of poetic manipulation built on subtle psychological schemes” (11). Let us try not to follow the manipulations of writers and interpreters, but instead let us treat Smerdyakov as an autonomous and gifted individual with consciousness. We would also like to question the possibility of Smerdyakov having committed a murder, especially from psychological and medical perspectives. Moreover, in our opinion Smerdyakov had no motive to kill Fyodor as he was the only person who showed Smerdyakov humane treatment. First, Smerdyakov’s social status was [...]

- **S3** score=0.0293 `karamazov-0429` — The Brothers Karamazov (Garnett) — Part II › Book V. Pro and Contra › Chapter II. Smerdyakov with a Guitar  
  “It’s all very well when you are firing at someone, but when he is firing straight in your mug, you must feel pretty silly. You’d be glad to run away, Marya Kondratyevna.” “You don’t mean you would run away?” But Smerdyakov did not deign to reply. After a moment’s silence the guitar tinkled again, and he sang again in the same falsetto: Whatever you may say, I shall go far away. Life will be bright and gay In the city far away. I shall not grieve, I shall not grieve at all, I don’t intend to grieve at all. Then something unexpected happened. Alyosha suddenly sneezed. They were silent. [...]

- **S4** score=0.0292 `karamazov-1177` — The Brothers Karamazov (Garnett) — Part IV › Book XI. Ivan › Chapter V. Not You, Not You!  
  He reached the gate of the house and had his hand on the bell, when he suddenly stopped. He felt that he was trembling all over with anger. Suddenly he let go of the bell, turned back with a curse, and walked with rapid steps in the opposite direction. He walked a mile and a half to a tiny, slanting, wooden house, almost a hut, where Marya Kondratyevna, the neighbor who used to come to Fyodor Pavlovitch’s kitchen for soup and to whom Smerdyakov had once sung his songs and played on the guitar, was now lodging. She had sold their little house, and was now living here with her mother. [...]

- **S5** score=0.0282 `karamazov-0182` — The Brothers Karamazov (Garnett) — Part I › Book III. The Sensualists › Chapter II. Lizaveta  
  Grigory rushed to Marfa and sent her to Lizaveta, while he ran to fetch an old midwife who lived close by. They saved the baby, but Lizaveta died at dawn. Grigory took the baby, brought it home, and making his wife sit down, put it on her lap. “A child of God—an orphan is akin to all,” he said, “and to us above others. Our little lost one has sent us this, who has come from the devil’s son and a holy innocent. Nurse him and weep no more.” So Marfa brought up the child. He was christened Pavel, to which people were not slow in adding Fyodorovitch (son of Fyodor). Fyodor Pavlovitch did not [...]

</details>

## q07 (single) — What secret did Mitya reveal about the money he spent at Mokroe, and why was he ashamed of it?
Retrieval: hit=1 recall=1.0 MRR=1.0 | abstained=False | cites gold=True | invalid citations=[]

**RAG answer:**
Mitya revealed that he spent only 1,500 roubles from Katerina Ivanovna’s 3,000 roubles, keeping the other 1,500 in a bag, which he later spent. He claimed he had not told anyone about the secret, though the prosecutor and others believed he had spread the rumor that he spent 3,000 roubles [S1][S4]. Mitya was ashamed because he felt a deep moral and emotional horror at having taken the money, especially given Katerina Ivanovna’s hatred of him and the fact that he had used it during a time of personal turmoil [S3][S4]. The prosecutor noted that the secrecy of the 1,500 roubles was "extremely surprising" and suggested it stemmed from a "positive horror" [S3]. Mitya’s shame was tied to his guilt over the deception and the emotional weight of his actions, not just the financial wrongdoing [S4].

**Cited:** [S1] The Brothers Karamazov (Garnett) — Part III › Book IX. The Preliminary Investigation › Chapter VII. Mitya’s Great Secret. Received with Hisses (`karamazov-0952`); [S3] The Brothers Karamazov (Garnett) — Part III › Book IX. The Preliminary Investigation › Chapter VII. Mitya’s Great Secret. Received with Hisses (`karamazov-0953`); [S4] The Brothers Karamazov (Garnett) — Part III › Book IX. The Preliminary Investigation › Chapter VII. Mitya’s Great Secret. Received with Hisses (`karamazov-0951`)

**Closed-book answer (no retrieval):**
(not run)

<details><summary>Retrieved passages</summary>

- **S1** score=0.0328 `karamazov-0952` — The Brothers Karamazov (Garnett) — Part III › Book IX. The Preliminary Investigation › Chapter VII. Mitya’s Great Secret. Received with Hisses  
  “Excuse me. How’s that? Why, when you were here a month ago you spent three thousand, not fifteen hundred, everybody knows that.” “Who knows it? Who counted the money? Did I let anyone count it?” “Why, you told everyone yourself that you’d spent exactly three thousand.” “It’s true, I did. I told the whole town so, and the whole town said so. And here, at Mokroe, too, everyone reckoned it was three thousand. Yet I didn’t spend three thousand, but fifteen hundred. And the other fifteen hundred I sewed into a little bag. That’s how it was, gentlemen. That’s where I got that money yesterday. [...]

- **S2** score=0.0315 `karamazov-0949` — The Brothers Karamazov (Garnett) — Part III › Book IX. The Preliminary Investigation › Chapter VI. The Prosecutor Catches Mitya  
  “Very well!” he exclaimed suddenly. “I will tell you my secret. I’ll tell you where I got the money! … I’ll reveal my shame, that I may not have to blame myself or you hereafter.” “And believe me, Dmitri Fyodorovitch,” put in Nikolay Parfenovitch, in a voice of almost pathetic delight, “that every sincere and complete confession on your part at this moment may, later on, have an immense influence in your favor, and may, indeed, moreover—” But the prosecutor gave him a slight shove under the table, and he checked himself in time. Mitya, it is true, had not heard him.

- **S3** score=0.0311 `karamazov-0953` — The Brothers Karamazov (Garnett) — Part III › Book IX. The Preliminary Investigation › Chapter VII. Mitya’s Great Secret. Received with Hisses  
  “I told no one.” “That’s strange. Do you mean absolutely no one?” “Absolutely no one. No one and nobody.” “What was your reason for this reticence? What was your motive for making such a secret of it? To be more precise: You have told us at last your secret, in your words, so ‘disgraceful,’ though in reality—that is, of course, comparatively speaking—this action, that is, the appropriation of three thousand roubles belonging to someone else, and, of course, only for a time is, in my view at least, only an act of the greatest recklessness and not so disgraceful, when one takes into [...]

- **S4** score=0.0302 `karamazov-0951` — The Brothers Karamazov (Garnett) — Part III › Book IX. The Preliminary Investigation › Chapter VII. Mitya’s Great Secret. Received with Hisses  
  “Yes, of course.” “I know you know her. She’s a noble creature, noblest of the noble. But she has hated me ever so long, oh, ever so long … and hated me with good reason, good reason!” “Katerina Ivanovna!” Nikolay Parfenovitch exclaimed with wonder. The prosecutor, too, stared. “Oh, don’t take her name in vain! I’m a scoundrel to bring her into it. Yes, I’ve seen that she hated me … a long while. … From the very first, even that evening at my lodging … but enough, enough. You’re unworthy even to know of that. No need of that at all. … I need only tell you that she sent for me a month [...]

- **S5** score=0.0296 `karamazov-0964` — The Brothers Karamazov (Garnett) — Part III › Book IX. The Preliminary Investigation › Chapter VII. Mitya’s Great Secret. Received with Hisses  
  In despair he hid his face in his hands. “Don’t worry yourself so, Dmitri Fyodorovitch,” observed the prosecutor, “everything that is written down will be read over to you afterwards, and what you don’t agree to we’ll alter as you like. But now I’ll ask you one little question for the second time. Has no one, absolutely no one, heard from you of that money you sewed up? That, I must tell you, is almost impossible to believe.” “No one, no one, I told you so before, or you’ve not understood anything! Let me alone!” “Very well, this matter is bound to be explained, and there’s plenty of [...]

</details>

## q08 (single) — What was the jury's verdict at Mitya's trial?
Retrieval: hit=0 recall=0.0 MRR=0.0 | abstained=False | cites gold=False | invalid citations=[]

**RAG answer:**
The jury's verdict at Mitya's trial was that Mitya was condemned to ten years of penal servitude for having killed his father while attempting to steal money from him [S1][S3]. The decision leaves the observers in the courtroom split, with most male observers accepting it and women expressing skepticism, considering it a mistake [S1]. The judges do not believe Ivan’s claim that Smerdyakov committed the murder, as Ivan is in a state of extreme agitation [S3]. While the prosecution presents evidence pointing to Mitya, the defense argues there is no conclusive proof and suggests the murder may not have occurred at all [S4]. Thus, the verdict is accepted by the majority, though it is contested by some, including women in the courtroom and literary critics [S1][S4].

**Cited:** [S1] Osińska & Szejko (2021) — PDF p. 3 (`osinska2021-0004`); [S3] Osińska & Szejko (2021) — PDF p. 3 (`osinska2021-0003`); [S4] Osińska & Szejko (2021) — PDF p. 14 (`osinska2021-0026`)

**Closed-book answer (no retrieval):**
(not run)

<details><summary>Retrieved passages</summary>

- **S1** score=0.0328 `osinska2021-0004` — Osińska & Szejko (2021) — PDF p. 3  
  to the trial in a state of extreme agitation. Finally, Mitya is condemned to ten years of penal servitude for having killed his father whilst attempting to steal money from him. The decision of the jury leaves the observers in the courtroom split. The decision is accepted by most of the male observers, whilst women express their skepticism and consider this decision to be a mistake. “They seemed to fancy that it might be at once reconsidered and reversed” (3). To sum up, the scene of the murder is never described objectively in the novel. We only get to hear Smerdyakov’s version when he [...]

- **S2** score=0.0313 `namli2022-0020` — Namli (2022) — PDF p. 8  
  At this point the reader knows that Mitya has been unjustly accused of his father Fyodor’s murder and that he is about to be found guilty. Towards the end of the trial, Mitya decides to accept the verdict, or, rather, the suffering that the verdict entails. He maintains his innocence of Fyodor’s death but cries out that he is nonetheless guilty of wanting to kill Fyodor. He wishes now to suffer and be cleansed by suffering (Dostoevsky 1990, p. 509). Raskolnikov of Crime and Punishment can be detected here but in the guise of two protagonists: Ivan, who tries to live in accordance with [...]

- **S3** score=0.0299 `osinska2021-0003` — Osińska & Szejko (2021) — PDF p. 3  
  did not kill his father. Another witness, Gregory, a servant that followed Mitya, was seriously injured when hit on the head by him. During the trial, Gregory gives evidence that he saw that the front door of Fyodor’s house was open. This confession will be used against Mitya. A couple of minutes later, the open door was also seen by Marfa, Gregory’s wife, who was woken by her husband’s scream. The fourth person in the house of the old Karamazov on the night when Fyodor was killed is Pavel Smerdyakov, who (as Gregory and Marfa confirm) had a very severe epileptic attack at that moment. [...]

- **S4** score=0.0161 `osinska2021-0026` — Osińska & Szejko (2021) — PDF p. 14  
  Results According to psychological and psychiatric approaches, and to suggestions that appear in the text, it seems that the most probable murderer was Mitya Karamazov. Dostoyevsky himself deceives the reader and does not give a direct answer to the question of who killed the old Karamazov. The narrator in the novel is no longer considered as the objective depositor of the truth. The witnesses’ statements are contradictory, but when referring to Mitya’s odium, Alosha and Grushenka are subjective in their arguments. The majority of the testimonies indicate that Mitya was the killer, and [...]

- **S5** score=0.0159 `karamazov-1172` — The Brothers Karamazov (Garnett) — Part IV › Book XI. Ivan › Chapter V. Not You, Not You!  
  “She is suffering. Why do you … sometimes say things to her that give her hope?” Alyosha went on, with timid reproach. “I know that you’ve given her hope. Forgive me for speaking to you like this,” he added. “I can’t behave to her as I ought—break off altogether and tell her so straight out,” said Ivan, irritably. “I must wait till sentence is passed on the murderer. If I break off with her now, she will avenge herself on me by ruining that scoundrel tomorrow at the trial, for she hates him and knows she hates him. It’s all a lie—lie upon lie! As long as I don’t break off with her, she [...]

</details>

## q09 (single) — What does Alyosha ask the boys to remember in his speech after Ilusha's funeral?
Retrieval: hit=1 recall=1.0 MRR=1.0 | abstained=False | cites gold=True | invalid citations=[]

**RAG answer:**
Alyosha asks the boys to remember Ilusha and each other, specifically recalling how they once bullied him but later grew fond of him. He emphasizes remembering Ilusha’s bravery and kindness, especially his stand for his father’s honor, and urges them to remain kind, honest, and generous like Ilusha and Kolya. He also asks them to keep a place in their hearts for one another and for him, promising to remember each of them even after thirty years. This memory, he believes, will help prevent them from becoming cruel or cynical in the future [S1][S3][S4].

**Cited:** [S1] The Brothers Karamazov (Garnett) — Epilogue › Chapter III. Ilusha’s Funeral. The Speech at the Stone (`karamazov-1515`); [S3] The Brothers Karamazov (Garnett) — Epilogue › Chapter III. Ilusha’s Funeral. The Speech at the Stone (`karamazov-1518`); [S4] Namli (2022) — PDF p. 11 (`namli2022-0029`)

**Closed-book answer (no retrieval):**
(not run)

<details><summary>Retrieved passages</summary>

- **S1** score=0.0323 `karamazov-1515` — The Brothers Karamazov (Garnett) — Epilogue › Chapter III. Ilusha’s Funeral. The Speech at the Stone  
  Meantime they were strolling slowly along the path and suddenly Smurov exclaimed: “There’s Ilusha’s stone, under which they wanted to bury him.” They all stood still by the big stone. Alyosha looked and the whole picture of what Snegiryov had described to him that day, how Ilusha, weeping and hugging his father, had cried, “Father, father, how he insulted you,” rose at once before his imagination. A sudden impulse seemed to come into his soul. With a serious and earnest expression he looked from one to another of the bright, pleasant faces of Ilusha’s schoolfellows, and suddenly said to [...]

- **S2** score=0.0323 `karamazov-1519` — The Brothers Karamazov (Garnett) — Epilogue › Chapter III. Ilusha’s Funeral. The Speech at the Stone  
  “Yes, yes, forever, forever!” the boys cried in their ringing voices, with softened faces. “Let us remember his face and his clothes and his poor little boots, his coffin and his unhappy, sinful father, and how boldly he stood up for him alone against the whole school.” “We will remember, we will remember,” cried the boys. “He was brave, he was good!” “Ah, how I loved him!” exclaimed Kolya. “Ah, children, ah, dear friends, don’t be afraid of life! How good life is when one does something good and just!” “Yes, yes,” the boys repeated enthusiastically. “Karamazov, we love you!” a voice, [...]

- **S3** score=0.0315 `karamazov-1518` — The Brothers Karamazov (Garnett) — Epilogue › Chapter III. Ilusha’s Funeral. The Speech at the Stone  
  “That will be so, I understand you, Karamazov!” cried Kolya, with flashing eyes. The boys were excited and they, too, wanted to say something, but they restrained themselves, looking with intentness and emotion at the speaker. “I say this in case we become bad,” Alyosha went on, “but there’s no reason why we should become bad, is there, boys? Let us be, first and above all, kind, then honest and then let us never forget each other! I say that again. I give you my word for my part that I’ll never forget one of you. Every face looking at me now I shall remember even for thirty years. Just [...]

- **S4** score=0.0303 `namli2022-0029` — Namli (2022) — PDF p. 11  
  After the funeral and shortly before the memorial dinner at the family’s house, the children gather beside Ilyusha’s stone—a place that the boy liked and where he asked to be buried. All are sorrowful, and one of the boys asks Alexei about the point of religion and, more concretely, the tradition of eating after a burial—doesn’t it run completely counter to nature that those grieving should gather to eat pancakes? Alexei does not reply but stands and recalls how he has been told that at this very stone Ilyusha wept in despair at how one of the boys had humiliated his father. At this very [...]

- **S5** score=0.0303 `karamazov-1520` — The Brothers Karamazov (Garnett) — Epilogue › Chapter III. Ilusha’s Funeral. The Speech at the Stone  
  “Certainly we shall all rise again, certainly we shall see each other and shall tell each other with joy and gladness all that has happened!” Alyosha answered, half laughing, half enthusiastic. “Ah, how splendid it will be!” broke from Kolya. “Well, now we will finish talking and go to his funeral dinner. Don’t be put out at our eating pancakes—it’s a very old custom and there’s something nice in that!” laughed Alyosha. “Well, let us go! And now we go hand in hand.” “And always so, all our lives hand in hand! Hurrah for Karamazov!” Kolya cried once more rapturously, and once more the [...]

</details>

## q10 (cross-passage) — How does Smerdyakov's confession to Ivan contradict the prosecutor's account of the murder?
Retrieval: hit=1 recall=0.5 MRR=0.5 | abstained=False | cites gold=True | invalid citations=[]

**RAG answer:**
Smerdyakov's confession to Ivan contradicts the prosecutor's account by asserting that Ivan ordered the murder and that Smerdyakov acted as the executor of Ivan’s will, not as an independent killer. Smerdyakov claims Ivan desired his father’s death to gain control of the inheritance, suggesting a premeditated plan rather than a spontaneous act [S1][S4]. This directly opposes the prosecutor’s narrative, which frames the murder as a crime committed by Smerdyakov alone, with no evidence of Ivan’s involvement. Furthermore, Smerdyakov’s confession is made during a severe epileptic seizure and under ambiguous conditions, raising doubts about its reliability [S1]. The prosecutor, however, insists on Smerdyakov’s guilt based on circumstantial evidence and the prisoner’s accusation, while Smerdyakov’s own statement implicates Ivan, creating a conflict between the official narrative and the confession [S2][S3].

**Cited:** [S1] Osińska & Szejko (2021) — PDF p. 3 (`osinska2021-0003`); [S2] The Brothers Karamazov (Garnett) — Part IV › Book XII. A Judicial Error › Chapter XII. And There Was No Murder Either (`karamazov-1447`); [S3] The Brothers Karamazov (Garnett) — Part IV › Book XII. A Judicial Error › Chapter XII. And There Was No Murder Either (`karamazov-1446`); [S4] Osińska & Szejko (2021) — PDF p. 8 (`osinska2021-0013`)

**Closed-book answer (no retrieval):**
(not run)

<details><summary>Retrieved passages</summary>

- **S1** score=0.0318 `osinska2021-0003` — Osińska & Szejko (2021) — PDF p. 3  
  did not kill his father. Another witness, Gregory, a servant that followed Mitya, was seriously injured when hit on the head by him. During the trial, Gregory gives evidence that he saw that the front door of Fyodor’s house was open. This confession will be used against Mitya. A couple of minutes later, the open door was also seen by Marfa, Gregory’s wife, who was woken by her husband’s scream. The fourth person in the house of the old Karamazov on the night when Fyodor was killed is Pavel Smerdyakov, who (as Gregory and Marfa confirm) had a very severe epileptic attack at that moment. [...]

- **S2** score=0.0315 `karamazov-1447` — The Brothers Karamazov (Garnett) — Part IV › Book XII. A Judicial Error › Chapter XII. And There Was No Murder Either  
  “It’s true, indeed, Smerdyakov is accused only by the prisoner, his two brothers, and Madame Svyetlov. But there are others who accuse him: there are vague rumors of a question, of a suspicion, an obscure report, a feeling of expectation. Finally, we have the evidence of a combination of facts very suggestive, though, I admit, inconclusive. In the first place we have precisely on the day of the catastrophe that fit, for the genuineness of which the prosecutor, for some reason, has felt obliged to make a careful defense. Then Smerdyakov’s sudden suicide on the eve of the trial. Then the [...]

- **S3** score=0.0297 `karamazov-1446` — The Brothers Karamazov (Garnett) — Part IV › Book XII. A Judicial Error › Chapter XII. And There Was No Murder Either  
  “But we shall be told at once again, ‘There is his father’s corpse! If he ran away without murdering him, who did murder him?’ Here, I repeat, you have the whole logic of the prosecution. Who murdered him, if not he? There’s no one to put in his place. “Gentlemen of the jury, is that really so? Is it positively, actually true that there is no one else at all? We’ve heard the prosecutor count on his fingers all the persons who were in that house that night. They were five in number; three of them, I agree, could not have been responsible—the murdered man himself, old Grigory, and his [...]

- **S4** score=0.0294 `osinska2021-0013` — Osińska & Szejko (2021) — PDF p. 8  
  All these arguments point against Smerdyakov being the potential killer of Fyodor Karamazov. As mentioned, old Karamazov was probably Pavel’s father, although he had never confirmed his paternity. Moreover, old Karamazov was the only person supporting him. He was sent to Moscow to study and later was employed in the position of cook and lackey. Even though Smerdyakov occasionally made vulgar comments regarding Fyodor, he also trusted him. When Smerdyakov himself admits that he killed Fyodor (and his confession is the only proof that he committed the murder), he also suggests that Ivan [...]

- **S5** score=0.0292 `karamazov-1396` — The Brothers Karamazov (Garnett) — Part IV › Book XII. A Judicial Error › Chapter VIII. A Treatise on Smerdyakov  
  “But what do we see? As soon as he is arrested the prisoner instantly throws all the blame on Smerdyakov, not accusing him of being his accomplice, but of being himself the murderer. ‘He did it alone,’ he says. ‘He murdered and robbed him. It was the work of his hands.’ Strange sort of accomplices who begin to accuse one another at once! And think of the risk for Karamazov. After committing the murder while his accomplice lay in bed, he throws the blame on the invalid, who might well have resented it and in self-preservation might well have confessed the truth. For he might well have [...]

</details>

## q11 (paper) — Which disciplines do Osińska and Szejko combine to analyse Mitya and Smerdyakov?
Retrieval: hit=1 recall=1.0 MRR=1.0 | abstained=False | cites gold=True | invalid citations=[]

**RAG answer:**
Osińska and Szejko combine literature studies, psychology, and psychiatry to analyse Mitya and Smerdyakov [S1][S3][S2].

**Cited:** [S1] Osińska & Szejko (2021) — PDF p. 1 (`osinska2021-0000`); [S2] Osińska & Szejko (2021) — PDF p. 16 (`osinska2021-0030`); [S3] Osińska & Szejko (2021) — PDF p. 14 (`osinska2021-0026`)

**Closed-book answer (no retrieval):**
(not run)

<details><summary>Retrieved passages</summary>

- **S1** score=0.0323 `osinska2021-0000` — Osińska & Szejko (2021) — PDF p. 1  
  The Mystery of the Crime in Skotoprigonyevsk Plot Analysis of The Brothers Karamazov from the Perspective of Literature Studies, Psychology and Psychiatry Katarzyna Osińska1, Natalia Szejko2,3 1 – Institute of Slavic Studies, Polish Academy of Science, Warsaw, Poland 2 – Department of Bioethics, Medical University of Warsaw, Poland 3 – Department of Neurology, Medical University of Warsaw, Poland Abstract In this article, by focusing on the two main protagonists, Mitya Karamazov and Pavel Smerdyakov, we would like to analyze the murder of Fyodor Karamazov, which is the crucial event in [...]

- **S2** score=0.0315 `osinska2021-0030` — Osińska & Szejko (2021) — PDF p. 16  
  hundred years old because they lay the foundations for canonical interpretations of this character. Nevertheless, we could see Smerdyakov from another perspective: as a man who was constantly rejected by those around him, who was never recognized as a brother, and who was a sick and devastated man. That is why he gives his money to Ivan and commits suicide and, according to Zosima, there is no man unhappier than a man who commits suicide. It does not seem possible to reach a conclusion as to whether Smerdyakov is a killer or not. Nevertheless, the version set out in this paper is [...]

- **S3** score=0.0313 `osinska2021-0026` — Osińska & Szejko (2021) — PDF p. 14  
  Results According to psychological and psychiatric approaches, and to suggestions that appear in the text, it seems that the most probable murderer was Mitya Karamazov. Dostoyevsky himself deceives the reader and does not give a direct answer to the question of who killed the old Karamazov. The narrator in the novel is no longer considered as the objective depositor of the truth. The witnesses’ statements are contradictory, but when referring to Mitya’s odium, Alosha and Grushenka are subjective in their arguments. The majority of the testimonies indicate that Mitya was the killer, and [...]

- **S4** score=0.03 `osinska2021-0002` — Osińska & Szejko (2021) — PDF p. 2  
  only novel by Dostoyevsky that has a truly polyphonic ending (2). Therefore, it cannot be interpreted as finished. To begin with, we would like to recap some well-known facts from the novel. Fyodor Pavlovich Karamazov is a landowner who has three sons: Dmitri (also known as Mitya) from his first marriage, and Ivan and Alexey from his second marriage. He is probably also the father of the butler, Pavel Smerdyakov. Pavel Smerdyakov is the son of Lisaveta Smerdyakova, the local mad lady who wanders aimlessly around the city and is commonly considered ‘yuródivyya’, or ‘mad in Christ’. Old [...]

- **S5** score=0.0299 `osinska2021-0029` — Osińska & Szejko (2021) — PDF p. 15  
  Alosha, a former monk who believes in obedience and truthfulness, decides to plan Mitya’s escape, although this would require the destruction of his moral principles. At the same time, none of the brothers mention Smerdyakov. Not only is he ignored during his lifetime and even more frequently treated badly, despised or even hated, but also no one has mercy for him, even after suicide. It is also worth mentioning that Smerdyakov’s suicide was, for some interpreters (especially those interpreting from the perspective of Christianity), another reason to blame him. Meanwhile, when preaching, [...]

</details>

## q12 (paper) — How does the article on love, attention and teaching connect active love to Iris Murdoch's idea of attention?
Retrieval: hit=1 recall=1.0 MRR=1.0 | abstained=False | cites gold=True | invalid citations=[]

**RAG answer:**
The article connects Dostoevsky’s notion of active love to Iris Murdoch’s concept of attention by highlighting their shared emphasis on humble, patient, and non-judgmental engagement with others. Both involve a "just and loving gaze" directed toward individual realities, focusing on concrete, everyday experiences rather than abstract ideals [S1][S4]. Active love, as described by Father Zosima, is portrayed as a form of attentive work that is difficult, ongoing, and rooted in quiet, daily actions—mirroring Murdoch’s view of attention as an exercise of love that enables moral knowledge through active presence [S2][S4]. The article argues that both concepts reject rigid boundaries between reason, emotion, and action, and that learning occurs through sustained, attentive engagement rather than forced instruction [S4]. Thus, active love and Murdoch’s attention are seen as complementary frameworks for understanding moral and educational development [S3][S4].

**Cited:** [S1] Love, attention and teaching (2018) — PDF p. 7 (`love_teaching2018-0019`); [S2] Love, attention and teaching (2018) — PDF p. 4 (`love_teaching2018-0007`); [S3] Love, attention and teaching (2018) — PDF p. 2 (`love_teaching2018-0001`); [S4] Love, attention and teaching (2018) — PDF p. 9 (`love_teaching2018-0025`)

**Closed-book answer (no retrieval):**
(not run)

<details><summary>Retrieved passages</summary>

- **S1** score=0.0323 `love_teaching2018-0019` — Love, attention and teaching (2018) — PDF p. 7  
  Love, attention and education Iris Murdoch’s concept of attention, adapted from the work of Simone Weil (1997, 2001), provides a helpful starting point in exploring some of the broader educational implications of these ideas.1 Murdoch (2001) defines attention as a ‘just and loving gaze directed upon an individual reality’ (p. 33). Attention is the task of active moral agents; it is an exercise of love through which we come to know others (pp. 29, 41). Murdoch is interested not so much in abstract principles as in the concrete and the particular. For Murdoch, the individual is the centre [...]

- **S2** score=0.0323 `love_teaching2018-0007` — Love, attention and teaching (2018) — PDF p. 4  
  can be regarded as an educational text: a work that has at its centre an implied pedagogical theory. Drawing on the work of Iris Murdoch, I argue that the key to linking the different elements of the educational process together is attention. It is attention, I suggest, that lies at the heart of active love; it is attention that allows us to bridge reason, faith and feeling; and it is attention that provides a helpful starting point for rethinking pedagogical purposes and practices. The first section examines several passages in The Brothers Karamazov that address the theme of active [...]

- **S3** score=0.0313 `love_teaching2018-0001` — Love, attention and teaching (2018) — PDF p. 2  
  OPEN REVIEW OF EDUCATIONAL RESEARCH 2018, VOL. 5, NO. 1, 1–15 https://doi.org/10.1080/23265507.2017.1404434 Love, attention and teaching: Dostoevsky’s The Brothers Karamazov Peter Roberts University of Canterbury, Christchurch, New Zealand ARTICLE HISTORY Received 21 August 2017 Accepted 5 November 2017 KEYWORDS Dostoevsky; love; attention; literature; teaching ABSTRACT Fyodor Dostoevsky’s final novel, The Brothers Karamazov, is one of the most influential works of the nineteenth century. To date, however, the potential value of the book for educationists has been largely ignored. This [...]

- **S4** score=0.0313 `love_teaching2018-0025` — Love, attention and teaching (2018) — PDF p. 9  
  There are important connections between Dostoevsky’s notion of active love and Murdoch’s concept of attentive love. The theme of active love is evident throughout Dostoevsky’s post-imprisonment writings (cf. McReynolds, 2008) but finds its fullest elaboration in The Brothers Karamazov. Active love, as explained by Father Zosima, is a form of humble, patient attention to others. It is non-judgemental; it entails accepting others as we find them and acting with a sense of equanimity and openness in our dealings with them. Active love is not concerned with grand gestures but small moments [...]

- **S5** score=0.0308 `love_teaching2018-0034` — Love, attention and teaching (2018) — PDF p. 12  
  Both Murdoch’s notion of attention and Dostoevsky’s concept of active love allow us to think about pedagogical ‘acceptance’ and ‘resistance’ in a fresh light. Acceptance of a certain kind is necessary in the sense of allowing the process of watching and waiting to occur. We might even think of this as a form of submission. Attention in education cannot be forced. There is, as David Lewin (2014a) points out, an element of attention that ‘eludes the simple direction of the will’; ‘a moment of awareness that in some respects is prior to the engagement of intended concentration’ (p. 355). [...]

</details>

## q13 (paper) — Why does Namli describe the theology of suffering in The Brothers Karamazov as an anti-theodicy?
Retrieval: hit=1 recall=1.0 MRR=1.0 | abstained=False | cites gold=True | invalid citations=[]

**RAG answer:**
Namli describes the theology of suffering in *The Brothers Karamazov* as an anti-theodicy because Ivan Karamazov, the novel’s central figure in this debate, rejects the idea that suffering can be justified by divine purpose or moral order. Ivan argues that it is immoral to justify the suffering of innocent people, asserting that a just God would not allow such suffering to exist. This positions him as a proponent of radical anti-theodicy, challenging the Christian theological assumption that God permits suffering for a greater good [S1][S4][S5]. Namli sees this as a normative critique of Christian morality, where Ivan’s nihilism stems from an honest confrontation with suffering’s meaning, leading him to revolt against God rather than accept a world of unjust pain [S3][S4]. Thus, the novel’s theology of suffering is not a solution to suffering but a rejection of traditional theodicy, emphasizing human agency and moral responsibility in the face of suffering.

**Cited:** [S1] Namli (2022) — PDF p. 1 (`namli2022-0000`); [S3] Namli (2022) — PDF p. 2 (`namli2022-0002`); [S4] Namli (2022) — PDF p. 6 (`namli2022-0013`); [S5] Namli (2022) — PDF p. 4 (`namli2022-0007`)

**Closed-book answer (no retrieval):**
(not run)

<details><summary>Retrieved passages</summary>

- **S1** score=0.0328 `namli2022-0000` — Namli (2022) — PDF p. 1  
  Studies in East European Thought (2022) 74:19–36 https://doi.org/10.1007/s11212-021-09454-x The Brothers Karamazov and the theology of suffering Elena Namli1 Accepted: 6 November 2021 / Published online: 17 January 2022 © The Author(s) 2022 Abstract This article offers a reflection upon The Brothers Karamazov, interpreted as a theological and philosophical contribution to the debate over humanity’s practical relationship to suffering and vulnerability. The relationship is practical insofar as the questions with which Dostoevsky struggles all relate to human agency: How should we live in [...]

- **S2** score=0.0313 `namli2022-0003` — Namli (2022) — PDF p. 2  
  Because the youngest brother Alexei, in my account of the novel, represents Dostoevsky’s embodiment of the gospel and a Christian “theology of suffering”, I will be paying especially close attention to Alexei’s relation to suffering. As will be seen, Alexei reconciles himself with a God who lacks the power to save humanity from suffering. At first, Alexei has no answer to his brother Ivan’s “damned questions” (prokliatye voprosy) about God and the meaning of suffering but decides to live as if all guilt—guilt before all and for all—is his alone. This decision leads Alexei to a kind of [...]

- **S3** score=0.0313 `namli2022-0002` — Namli (2022) — PDF p. 2  
  This essay offers a reflection upon Dostoevsky’s final novel, The Brothers Karamazov, which I read as a theological and philosophical contribution to the debate over humanity’s practical relationship to suffering and its own vulnerability. The relationship is practical insofar as the questions with which Dostoevsky struggles all relate to human agency: How should we live in the continual presence of suffering? How should a Christian live in a world in which innocent people and animals are tormented while evil people live contentedly? My aim is to reconstruct a theology of suffering in [...]

- **S4** score=0.0312 `namli2022-0013` — Namli (2022) — PDF p. 6  
  Hitherto my argument has been that The Brothers Karamazov is a novel about practical reason—how we should live in a world full of suffering, not how we should understand that world. But The Brothers Karamazov is also a book about the implications of Christian faith for the positions adopted by people in practice, and for this reason Ivan and his brothers’ struggle with the insight granted by reason into the meaningless of life becomes a struggle over Christianity’s image of God. Of all the brothers, it falls to Ivan to fight this battle in relation to the closely proximate issue of [...]

- **S5** score=0.0303 `namli2022-0007` — Namli (2022) — PDF p. 4  
  In light of all this, I read the novel as an engagement with precisely this question of what it means for a Christian to take doubt and truth seriously. The novel presents various practical approaches to suffering and death in how the brothers, just like their doubles (Namli 2009, pp. 56–57), not only meditate on but also live with these damned questions. Ivan Ivan, Fyodor Karamazov’s son by his second wife, distinguishes himself from his brothers by his talent and academic education. In the novel, Ivan represents the challenge posed by nihilism to Christianity and, in particular, what [...]

</details>

## q14 (paper) — Which other novels does Admirand compare with The Brothers Karamazov when discussing theist–atheist encounters?
Retrieval: hit=1 recall=1.0 MRR=1.0 | abstained=False | cites gold=True | invalid citations=[]

**RAG answer:**
Admirand compares *The Brothers Karamazov* with *Les Misérables* and *The Plague* when discussing theist–atheist encounters [S1][S4][S5]. These three novels are examined as examples of fictional dialogues between theist and atheist characters, offering insights into contemporary theist–atheist dialogue [S1][S4].

**Cited:** [S1] Admirand (2021) — PDF p. 1 (`admirand2021-0000`); [S4] Admirand (2021) — PDF p. 2 (`admirand2021-0004`); [S5] Admirand (2021) — PDF p. 11 (`admirand2021-0038`)

**Closed-book answer (no retrieval):**
(not run)

<details><summary>Retrieved passages</summary>

- **S1** score=0.0328 `admirand2021-0000` — Admirand (2021) — PDF p. 1  
  religions Article Theist–Atheist Encounters in Les Misérables, The Brothers Karamazov, and The Plague Peter Admirand School of Theology, Philosophy, and Music, DCU All Hallows Campus, Dublin City University, Dromcondra, Dublin 9, Ireland; peter.admirand@dcu.ie Abstract: Turning to the novels, Les Misérables, The Brothers Karamazov, and The Plague, this article focuses on theist–atheist encounters within ﬁction as guides and challenges to contemporary atheist– theist dialogue. It ﬁrst provides a discussion of deﬁnitions pertinent to our topic and a reﬂection on the value and limitations [...]

- **S2** score=0.0323 `admirand2021-0005` — Admirand (2021) — PDF p. 2  
  disparaging claims of Dostoevsky’s prose as “deliberately repetitious, ﬂat, low key”, are not uncommon.11 My reasons for examining these three otherwise acclaimed novels are mostly personal. While at The Catholic University of America in the mid-nineties, I was introduced to Dostoevsky’s The Brothers Karamazov through Professor Declan’s honours seminar and in his book, After Ideology: Recovering the Spiritual Foundations of Freedom, while Professor Stephen Schneck encouraged close philosophical reading of The Plague for an ethics and politics class. As Camus so closely read Dostoevsky, [...]

- **S3** score=0.0306 `admirand2021-0020` — Admirand (2021) — PDF p. 6  
  Turning to the novelists, it is not surprising, then, that even as I continue to work in the area of theist–atheist dialogue with fellow ﬂesh-and-blood human beings, I also 46 (Bullivant and Ruse 2014; Crane 2017). For an analysis of atheist writers critical of the New Atheists, see (Admirand 2020a). 47 See, for example, (Admirand and Fiala 2019). 48 (Dalai Lama 2011; Dalai Lama and Alt 2017). 49 (Dalai Lama 2010, p. 109). 50 See, for example, (Peace et al. 2012); in postconﬂict contexts, see (Admirand 2020b). 51 (Oz 2005). 52 See, for example, (Admirand 2020c). 53 The best place to [...]

- **S4** score=0.0301 `admirand2021-0004` — Admirand (2021) — PDF p. 2  
  as zeal for the thesis has cooled, the so-called European exceptions, such as Ireland and Poland, have seen great growth in the number of nones or those unchurched.6 So, too is there an increase in multiple religious belonging in the West, a feature traditionally aligned with the East.7 Regardless, human identity and longing for what are deemed religious or transcendental forms of belief and belonging, whether in traditionally religious or secular leanings, remain universal in scope.8 This article is focused on moments of private discussion and dialogue between two characters in novels, [...]

- **S5** score=0.029 `admirand2021-0038` — Admirand (2021) — PDF p. 11  
  For our purposes, we will examine (though brieﬂy) the well-known debate/dialogues about God and theodicy between Alyosha and Ivan, again focusing on challenges and lessons depicted in this believer–nonbeliever dialogue. It should be stressed that, much like Hugo, Dostoevsky was also a theist, but more so than Hugo, deeply feared what he saw as a nihilistic surge through Europe rooted in a turning away from God and traditional religious belief. Alyosha, deemed by Dostoevsky as the hero of the novel precisely for his stance and hope for God, was named after one of Dostoevsky’s sons who [...]

</details>

## q15 (cross-doc) — How do Gabor and Namli each interpret Zosima's response to Ivan's argument about suffering?
Retrieval: hit=1 recall=0.5 MRR=1.0 | abstained=True | cites gold=False | invalid citations=[]

**RAG answer:**
The provided sources do not contain enough information to answer this. The question asks for interpretations by both Gabor and Namli, but only Gabor is cited in the sources. There is no mention of Namli or their interpretation of Zosima's response. Therefore, it is impossible to provide a comparative answer as requested.

**Cited:** none

**Closed-book answer (no retrieval):**
(not run)

<details><summary>Retrieved passages</summary>

- **S1** score=0.0323 `gabor2024-0010` — Gabor (2024) — PDF p. 5  
  In our context, Ivan’s description of the world denies Zosima’s, but Zosima’s does not contradict Ivan’s. Instead, it embraces it. The result is that the world of suffering is no longer denied; a heavenly life can take place in the middle of suffering, as long as you share it with someone else. The famous chapter “Rebellion” begins with Ivan’s statement about the impossibility of love. “I could never understand how one could love one’s neighbor. In my opinion, it’s precisely those who are near us that it is impossible to love, and one can only love those who are distant from us.”17 Then [...]

- **S2** score=0.0323 `gabor2024-0029` — Gabor (2024) — PDF p. 14  
  Zosima’s perspective embraces all people, including Ivan. And, what may sound outrageous, it also includes the general who murdered the child before his mother’s eyes. This is because, just as in the unilateral contradiction that Constantin Noica theorizes, evil may reject the good, but the good embraces it. Dostoevsky’s approach in The Karamazov Brothers is to show that the suffering of the world is indeed incomprehensible. Attempting any kind of theodicy is a disservice to God and humanity. Suffering is never justified. Nevertheless, suffering is present. A heavenly existence is not [...]

- **S3** score=0.0308 `gabor2024-0014` — Gabor (2024) — PDF p. 7  
  mother’s very eyes, the child was hunted down and torn to pieces by the dogs!27 What should people do with him, Ivan asks? Shot him? And Alyosha answers, “Yes, shot him.” Alyosha’s answer sounds logical in the context of justice, which requires one to receive one’s reward for one’s actions. But Alyosha acknowledges it as an absurd response because it is given within an absurd world. This absurd world demands explanations that make sense within its framework. Evil can stand only within the space that denies the possibility of good. Book VI reveals that from the outside of this space, evil [...]

- **S4** score=0.0308 `gabor2024-0026` — Gabor (2024) — PDF p. 13  
  he is one of the ingredients, that the soup precedes him, and it precedes him with its own pains and sorrows. But now, that he is alive, its pains and sorrows are also part of his body; its taste is also due to him, to his inability to work in synergy with others, the other carrots and tomatoes of this soup. Grushenka’s love, the anonymous embrace he received with a pillow, and the complete humility to which he was brought gave birth in him to a love that he had forgotten: he is responsible for all, and he is so in love. The call is to embrace others, and not to refuse responsibility for [...]

- **S5** score=0.0299 `gabor2024-0000` — Gabor (2024) — PDF p. 1  
  The Problem of Evil and Fr. Zosima’s Responsibility Before All Octavian Gabor* Ivan’s exposition of the problem of evil in Dostoevsky’s The Brothers Karamazov is often described as one of the most powerful defenses of the idea that the amount and the radical nature of unexplained evil are inconsistent with the existence of God. James Scanlan calls it “one of the most gripping statements of the philosophical «problem of evil» in world literature.”¹ Anthologies used for introductory courses in philosophy don’t fail to include Ivan’s indictment of God, and such anthologies are not famous [...]

</details>

## q16 (cross-doc) — What does the Grand Inquisitor claim in the novel, and how does Admirand interpret that chapter?
Retrieval: hit=1 recall=1.0 MRR=1.0 | abstained=False | cites gold=True | invalid citations=[]

**RAG answer:**
The Grand Inquisitor claims that humanity does not desire freedom but instead craves happiness through security, "bread and circuses," and authority—specifically, the stability provided by a divine, authoritarian order. He argues that moral freedom is a burden, and that people prefer a world of "mystery, miracle, and authority" over the chaos of choice (S4). He sees the Church as having corrected Christ’s rejection of temptation by embracing earthly power and control (S4).  

Admirand interprets this as a critique of totalitarianism, drawing parallels to Juvenal’s "bread and circuses," Maoist China, and modern political systems (S2). They note the Inquisitor’s portrayal of Jesus as compassionate and silent, emphasizing a gentle, forgiving figure in contrast to traditional iconography (S2). Admirand also sees Dostoevsky’s Jesus as aligned with liberation theology and a kind, forgiving Christ, reflecting a Catholic theological vision rooted in love and faith (S2).

**Cited:** [S2] Admirand (2021) — PDF p. 14 (`admirand2021-0049`); [S4] Love, attention and teaching (2018) — PDF p. 6 (`love_teaching2018-0014`)

**Closed-book answer (no retrieval):**
(not run)

<details><summary>Retrieved passages</summary>

- **S1** score=0.0307 `karamazov-0475` — The Brothers Karamazov (Garnett) — Part II › Book V. Pro and Contra › Chapter V. The Grand Inquisitor  
  The procession halts, the coffin is laid on the steps at His feet. He looks with compassion, and His lips once more softly pronounce, ‘Maiden, arise!’ and the maiden arises. The little girl sits up in the coffin and looks round, smiling with wide-open wondering eyes, holding a bunch of white roses they had put in her hand. “There are cries, sobs, confusion among the people, and at that moment the cardinal himself, the Grand Inquisitor, passes by the cathedral. He is an old man, almost ninety, tall and erect, with a withered face and sunken eyes, in which there is still a gleam of light. [...]

- **S2** score=0.0303 `admirand2021-0049` — Admirand (2021) — PDF p. 14  
  The Inquisitor’s claims are not new. They echo Juvenal’s phrase of “bread and circuses” given to Roman citizens to appease them. They also resonate with similar phrases in later Maoist China and with a China economically strong today but still hiding past failures like the Great Chinese Famine.93 Just as Jesus would be a threat in such 20th century totalitarian regimes, he is arrested in 16th century theocratic Spain. Throughout the Grand Inquisitor’s narrative, Jesus says nothing. His only reply is to “gently” kiss the Grand Inquisitor on the lips, resembling Judas’ betrayal of Jesus [...]

- **S3** score=0.0296 `karamazov-0496` — The Brothers Karamazov (Garnett) — Part II › Book V. Pro and Contra › Chapter V. The Grand Inquisitor  
  Alyosha had listened in silence; towards the end he was greatly moved and seemed several times on the point of interrupting, but restrained himself. Now his words came with a rush. “But … that’s absurd!” he cried, flushing. “Your poem is in praise of Jesus, not in blame of Him—as you meant it to be. And who will believe you about freedom? Is that the way to understand it? That’s not the idea of it in the Orthodox Church. … That’s Rome, and not even the whole of Rome, it’s false—those are the worst of the Catholics, the Inquisitors, the Jesuits! … And there could not be such a fantastic [...]

- **S4** score=0.0294 `love_teaching2018-0014` — Love, attention and teaching (2018) — PDF p. 6  
  actions come to the attention of the Grand Inquisitor, a ninety year old Roman Catholic Cardinal, who has sanctioned the burning of dozens of heretics just prior to Christ’s arrival. The Grand Inquisitor summons Christ to his cell and admonishes the latter for disrupting order in the town. Motivated by his love for humankind, the Grand Inquisitor advises Christ that he too will have to be put to death. The people may praise him today, the Grand Inquisitor says to Christ, but tomorrow they could just as easily turn on him and call for his blood. Through Christ, people are granted moral [...]

- **S5** score=0.0291 `admirand2021-0046` — Admirand (2021) — PDF p. 13  
  Alyosha, does, though, bring up Jesus, and his sacriﬁce and atonement. Ivan tells him he was building towards Jesus and so tells the story of “The Grand Inquisitor”. As Frank Armstrong comments, through Ivan and the Grand Inquisitor story, “Dostoyevsky is voicing his deep animosity to Catholicism, the Jesuit order in particular and the conﬂation of religious with temporal power generally”.86 According to Gary Adelman, Dostoevsky also “poured his extreme life-hatred of Jews . . . into the Grand Inquisitor, quite consciously attacking in him the Jew in his own imagination”.87 Antonio Malo, [...]

</details>

## q17 (unanswerable) — How many copies did the first edition of The Brothers Karamazov sell?
Retrieval: hit=None recall=None MRR=None | abstained=True | cites gold=None | invalid citations=[]

**RAG answer:**
The provided sources do not contain enough information to answer this. None of the sources mention the number of copies sold by the first edition of The Brothers Karamazov.

**Cited:** none

**Closed-book answer (no retrieval):**
(not run)

<details><summary>Retrieved passages</summary>

- **S1** score=0.0328 `gabor2024-0011` — Gabor (2024) — PDF p. 5  
  17 Fyodor Dostoevsky, The Karamazov Brothers. Trans. by Ignat Avsey (Oxford: University Press, 2008), 296. All quotes from The Karamazov Brothers are from this edition.

- **S2** score=0.0161 `karamazov-0557` — The Brothers Karamazov (Garnett) — Part II › Book VI. The Russian Monk › Chapter I. Father Zossima and His Visitors  
  There’s no need to build halls for this, let him take them into his own cottage. They won’t spoil his cottage, they would only be there one hour. Let him open that book and begin reading it without grand words or superciliousness, without condescension to them, but gently and kindly, being glad that he is reading to them and that they are listening with attention, loving the words himself, only stopping from time to time to explain words that are not understood by the peasants. Don’t be anxious, they will understand everything, the orthodox heart will understand all! Let him read them [...]

- **S3** score=0.0161 `admirand2021-0034` — Admirand (2021) — PDF p. 10  
  The Brothers Karamazov was published in 1881, so almost three decades after his release, and one year before his death in 1882. In the novel, Fyodor Karamazov, the father, is described as a landowner who is “not only worthless and depraved but muddleheaded as well” (7). He only thought of himself. He was an “old fool” (74). As the opening of the novel reveals, the father had died 13 years previously. As the story unfolds, the question is which of his sons killed him, for any one of them had motive. Fyodor Karamazov, it is worth noting, was said to be modelled after Dostoevsky’s own [...]

- **S4** score=0.0159 `karamazov-0141` — The Brothers Karamazov (Garnett) — Part I › Book II. An Unfortunate Gathering › Chapter VII. A Young Man Bent on a Career  
  “You are mistaken about that woman. Dmitri—despises her,” said Alyosha, with a sort of shudder. “Grushenka? No, brother, he doesn’t despise her. Since he has openly abandoned his betrothed for her, he doesn’t despise her. There’s something here, my dear boy, that you don’t understand yet. A man will fall in love with some beauty, with a woman’s body, or even with a part of a woman’s body (a sensualist can understand that), and he’ll abandon his own children for her, sell his father and mother, and his country, Russia, too. If he’s honest, he’ll steal; if he’s humane, he’ll murder; if [...]

- **S5** score=0.0159 `love_teaching2018-0002` — Love, attention and teaching (2018) — PDF p. 2  
  Fyodor Dostoevsky’s final novel, The Brothers Karamazov (Dostoevsky, 1991), is almost universally acknowledged as his masterpiece. It has, in Joseph Frank’s words, a ‘grandeur’ that evokes comparison with ‘the greatest creations of Western literature’ (Frank, 2002, p. 567). Richard Neuhaus has described The Brothers Karamazov as ‘the greatest novel ever written’, noting that it is the one book he returns to year after year, ‘always with increased pleasure and admiration’ (Neuhaus, 2003, p. 75). Others have referred to the book as ‘the greatest Christian novel ever written’ (Delasanta, [...]

</details>

## q18 (unanswerable) — What happens to Mitya after he escapes to America?
Retrieval: hit=None recall=None MRR=None | abstained=True | cites gold=None | invalid citations=[]

**RAG answer:**
The provided sources do not contain enough information to answer this. While Mitya considers escaping to America and expresses strong negative feelings about it—calling it "a bad exile as bad, perhaps, as Siberia" and hating the idea—he does not describe what actually happens to him after he escapes. The sources indicate his internal conflict, his desire to escape, and his belief that Grushenka will suffer for him, but there is no narrative account of his life or fate in America. The question of what happens to Mitya after such an escape is not addressed in the given texts.

**Cited:** none

**Closed-book answer (no retrieval):**
(not run)

<details><summary>Retrieved passages</summary>

- **S1** score=0.0315 `namli2022-0020` — Namli (2022) — PDF p. 8  
  At this point the reader knows that Mitya has been unjustly accused of his father Fyodor’s murder and that he is about to be found guilty. Towards the end of the trial, Mitya decides to accept the verdict, or, rather, the suffering that the verdict entails. He maintains his innocence of Fyodor’s death but cries out that he is nonetheless guilty of wanting to kill Fyodor. He wishes now to suffer and be cleansed by suffering (Dostoevsky 1990, p. 509). Raskolnikov of Crime and Punishment can be detected here but in the guise of two protagonists: Ivan, who tries to live in accordance with [...]

- **S2** score=0.0293 `karamazov-1496` — The Brothers Karamazov (Garnett) — Epilogue › Chapter II. For a Moment the Lie Becomes Truth  
  I must tell you the truth. And so I can’t judge of your own action. But let me assure you that I shall never condemn you. And it would be a strange thing if I could judge you in this. Now I think I’ve gone into everything.” “But I do condemn myself!” cried Mitya. “I shall escape, that was settled apart from you; could Mitya Karamazov do anything but run away? But I shall condemn myself, and I will pray for my sin forever. That’s how the Jesuits talk, isn’t it? Just as we are doing?” “Yes.” Alyosha smiled gently. “I love you for always telling the whole truth and never hiding anything,” [...]

- **S3** score=0.0164 `karamazov-1163` — The Brothers Karamazov (Garnett) — Part IV › Book XI. Ivan › Chapter IV. A Hymn and a Secret  
  I should only smash my skull with the hammer! But, on the other hand, my conscience? I should have run away from suffering. A sign has come, I reject the sign. I have a way of salvation and I turn my back on it. Ivan says that in America, ‘with the goodwill,’ I can be of more use than underground. But what becomes of our hymn from underground? What’s America? America is vanity again! And there’s a lot of swindling in America, too, I expect. I should have run away from crucifixion! I tell you, you know, Alexey, because you are the only person who can understand this. There’s no one else. [...]

- **S4** score=0.0164 `karamazov-0994` — The Brothers Karamazov (Garnett) — Part III › Book IX. The Preliminary Investigation › Chapter IX. They Carry Mitya Away  
  “I’ll trouble you, sir, to learn how to speak to me if you’ve never been taught. I’m not ‘old fellow’ to you, and you can keep your advice for another time!” Mavriky Mavrikyevitch snapped out savagely, as though glad to vent his wrath. Mitya was reduced to silence. He flushed all over. A moment later he felt suddenly very cold. The rain had ceased, but the dull sky was still overcast with clouds, and a keen wind was blowing straight in his face. “I’ve taken a chill,” thought Mitya, twitching his shoulders. At last Mavriky Mavrikyevitch, too, got into the cart, sat down heavily, and, as [...]

- **S5** score=0.0161 `karamazov-0995` — The Brothers Karamazov (Garnett) — Part III › Book IX. The Preliminary Investigation › Chapter IX. They Carry Mitya Away  
  Mitya had time to seize and press his hand. “Goodbye, dear fellow! I shan’t forget your generosity,” he cried warmly. But the cart moved and their hands parted. The bell began ringing and Mitya was driven off. Kalganov ran back, sat down in a corner, bent his head, hid his face in his hands, and burst out crying. For a long while he sat like that, crying as though he were a little boy instead of a young man of twenty. Oh, he believed almost without doubt in Mitya’s guilt. “What are these people? What can men be after this?” he exclaimed incoherently, in bitter despondency, almost [...]

</details>
