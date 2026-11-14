# DD2380 HT26 — Artificial Intelligence (11237)

> **Everything in the course, plus everything you owe it.**
> Snapshot: 2026-11-14 · Materials: `courses/DD2380_Artificial_Intelligence/`
> Canvas: https://canvas.kth.se/courses/65313

---

## 1. At a glance

| | |
|---|---|
| **Course code** | DD2380 (course instance 11237) |
| **Credits** | 6.0 hp |
| **Examiner / responsible** | André Pereira |
| **Other teachers** | Petter Ögren, Iolanda Leite, Noémie Jaquier |
| **Email** | rpl-ai-teachers@eecs.kth.se |
| **Language** | English — all submissions and exams |
| **Textbook** | Russell & Norvig, *Artificial Intelligence: A Modern Approach* (free via KTH Library) |
| **Kattis** | https://kth.kattis.com/courses/DD2380/ht26 |
| **Status right now** | 6 of 14 lectures done · Search classroom quiz graded · 3 programmming assignments all outstanding |

**Course components**

| Component | Credits | What it is | Grading |
|---|---|---|---|
| RAP1 | 0.5 | Ethics essay | Pass/Fail |
| TENQ | 1.5 | 6 Canvas quizzes + 3 on-campus quizzes | Pass/Fail |
| LAB2 | 4.0 | Search + HMM + RL programming assignments | A–F (**this sets your final grade**) |

To pass you must pass **all three**. The letter grade comes from LAB2 only.

---

## 2. Learning outcomes

After passing you should be able to:

1. Apply different principles of AI
2. Choose appropriate tools and implement efficient solutions to AI problems
3. Integrate tools to design programs with properties expected of an intelligent system
4. Present, analyse and justify your own solution to an AI problem
5. Reflect on and discuss current social and ethical aspects of AI

...so that you can use AI methods in analysis, design and implementation of software, and contribute to designing intelligent systems in academia and industry.

---

## 3. Lecture map (actual 2026 dates)

All lectures are in person, not recorded. Attendance optional, strongly recommended.

| # | Date (2026) | Topic | Textbook (Pearson 2013 / Global 2016) | Slides in folder |
|---|---|---|---|---|
| 0 | 29 Oct 08:00 | Intro + Practicalities | — | `L01 - Introduction and practicalities/` |
| 1 | 29 Oct 13:00 | Ethics | 1–2 / 1–2, 26–27 | `L02 - AI and Society (ethics)/` |
| 2 | 30 Oct 10:00 | Search | 3 / 3 | `L03-04 - Search and Games/` |
| 3 | 3 Nov 15:00 | Adversarial Search | 5 / 5 | `L03-04 - Search and Games/` |
| 4 | 4 Nov 10:00 | Logic and Planning | 6, 8–9, 10, 11 / 7–9, 10, 11 | `L05 - Knowledge, reasoning, planning/` |
| 5 | 9 Nov 10:00 | Probabilistic Reasoning | 13–15 / 13–15 | `L06-07 - Probabilistic reasoning and HMMs/` |
| **6** | **13 Nov 10:00** | **HMMs** | 13–15 / 13–15 | `L06-07 .../` |
| 7 | 19 Nov 13:00 | Decision Making | 16–17 / 16–17 | *(not yet posted)* |
| 8 | 23 Nov 08:00 | Reinforcement Learning | 23 / 21 | *(not yet posted)* |
| 9 | 26 Nov 08:00 | Multi-Agent Systems + Robotics | 25 / 25 | *(not yet posted)* |
| 10 | 2 Dec 10:00 | Machine Learning | 19 / 18 | *(not yet posted)* |
| 11 | 7 Dec 13:00 | NLP + Conversational Systems | 21, 23 / 22–23 | *(not yet posted)* |
| 12 | 10 Dec 08:00 | Computer Vision | 24 / 24 | *(not yet posted)* |
| 13 | 21 Dec 10:00 | Generative AI | — | *(not yet posted)* |

Plus **3 tutorials** (Search/Games, HMMs, RL) — each offered in multiple parallel slots, not compulsory, recommended if you want hands-on practice.

---

## 4. Everything you must do

### 4.1 Ethics essay (RAP1) — ⚠️ deadline passed 9 Nov

- Read several scientific papers
- Write an **individual reflection** on ethical/societal aspects of AI
- Discuss in a group of 3–4 (4 strongly preferred)
- Write a **summary of the group discussion**
- Group sign-up via People → Groups → "Essay group xxx" (use the pre-created ones, don't create your own)

Materials: `Lecture 2 - Intro to AI Ethics.pdf`, `EthicsCanvas.pdf`, `HazardsTable.pdf`, `Roboted.pdf`, `Robotsinsociety.pdf`

**Status: NOT submitted on Canvas.** Talk to the teaching team immediately — this is a Pass/Fail gate on the whole course.

### 4.2 Programming assignments (LAB2) — the grade decider

Each assignment = **Kattis submission** + **your own Assignment Learning Journal (PDF)**.

- Work in **pairs** (strongly encouraged) or alone. **Max 2 students.** No new partner if a pairing falls apart.
- Each student writes their **own** journal, even if code was shared.
- Team composition may differ between assignments.

**How the grade works**

| Kattis achievement | Grade range | Journal role |
|---|---|---|
| Part 1 passed | E – D | Distinguishes basic completion vs. strong explanation |
| Part 2 passed | C | Must show correct understanding of the advanced method |
| Part 3 passed | B – A | Distinguishes good solution vs. excellent analysis |

Passing a Kattis level sets the **ceiling**, not the grade. The journal decides within that range. **To get an A, both code and journal must be on time.**

#### Search — due **23 Nov 2026, 19:00**
- Topic: classical and adversarial search — informed search + game-tree search
- Submit to Kattis: *Fishing Derby: Search*
- Files: `Assignments/DD2380_2026_Search_Assignment.pdf`, `..._skeleton.zip` (already extracted), `Search_Tutorial.pdf`, `Lecture 3 - Search.pdf`, `Lecture 4 - Adversarial Search.pdf`
- Kattis has 3 cumulative parts

#### HMM — due **30 Nov 2026, 19:00**
- Topic: reasoning under uncertainty, Hidden Markov Models
- Kattis tasks: HMM0, HMM1, HMM2, HMM3, + Fishing Derby (for B–A)
- Data: `hmm_c_N1000.in` (grade C investigation), `hmm_c_N10000.in`
- Skeleton: `fishingderby_hmm.zip` (already extracted)
- Journal structure: **J0–J6**
- Files: `Assignments/DD2380 2026 HMM Assignment`, `HMM_tutorial.pdf`, `Tutorial_HMM1_exercise_forward.pdf`, `Tutorial_HMM2_exercise_viterbi.pdf`, `HMM tutorial by Stamp.pdf`

#### RL — due **7 Dec 2026, 19:00**
- Topic: reinforcement learning — agents that learn through interaction
- Unlocked 23 Nov 09:00 · Assignment files not yet posted

> ⚠️ **All three deadlines are strict, no extensions.** Late submission of any required component → max LAB2 grade of B. Aim to submit everything 2 days early.

### 4.3 Quizzes (TENQ) — online part

6 Canvas quizzes. Threshold **60%**. 60 minutes per attempt, 5 attempts allowed, all close **8 Jan 2027, 19:00**.

| Quiz | Unlocks | Status |
|---|---|---|
| Q0: Code of conduct | 27 Oct 08:30 | ⬜ |
| Q1: Logic & Planning | 4 Nov 12:00 | ⬜ |
| Q2: Robotics and Multi-agent Systems | 26 Nov 10:00 | ⬜ |
| Q3: Machine Learning | 2 Dec 12:00 | ⬜ |
| Q4: NLP and Conversational AI | 7 Dec 15:00 | ⬜ |
| Q5: Computer Vision | 10 Dec 10:00 | ⬜ |

### 4.4 Quizzes (TENQ) — on-campus part

3 classroom quizzes, one per assignment topic. **50%** to pass. 50 minutes each, **4 time slots each** — sign up in the Canvas Calendar.

| Quiz | Status |
|---|---|
| Classroom Quiz: Search (10 Nov) | ✅ **Graded — 3.0 points, passed** |
| Classroom Quiz: HMM | ⬜ 4 slots, sign up |
| Classroom Quiz: RL | ⬜ 4 slots, sign up |

### 4.5 Individual oral examination (Redovisning)

- **One 30-minute slot**, booked from the Canvas calendar (after 7 Dec).
- At the start, **one of Search / HMM / RL is picked for you at random, independently per student.**
- You must explain: the theory, your Learning Journal, your implementation, design choices, results, limitations.
- It does **not** change individual assignment grades — it sets an **individual cap on LAB2**.
  - E.g. average suggests A, but you show C-level understanding → LAB2 capped at C.
  - Can't demonstrate understanding at all → cap can be **F**, and you fail LAB2 despite passing Kattis.

**Practical implication:** you must genuinely understand all three implementations. Don't let a partner write code you can't explain.

---

## 5. Grading criteria detail

To reach a level you must satisfy that level's criteria **and all lower levels**.

**ILO 1 — Apply AI principles**
- E: apply basic concepts, modelling techniques, algorithms, tools across all course topics
- C: apply more *advanced* concepts across all topics

**ILO 2 — Choose tools, implement efficient solutions**
- E: solve selected AI sub-problems at a basic level by implementing and debugging given algorithms
- C: propose and implement simple modifications based on evaluating weaknesses in your own implementation
- A: solve problems significantly outperforming basic solutions by selecting, implementing, combining and fine-tuning algorithms **under limited resources**

**ILO 3 — Integrate tools for intelligent-system properties**
- E: design a program that can predict, make decisions, or improve over time

**ILO 4 — Present, analyse, justify own solution**
- E: clearly explain implementation details, algorithm principles, and why the algorithm suits the problem

**ILO 5 — Reflect on social/ethical aspects**
- Assessed by the ethics essay

---

## 6. Course rules & practicalities

- **Not fully virtual.** Lectures, tutorials, on-campus quizzes and oral exams are in person. Only Canvas quizzes are online.
- **Recordings:** none, unless a session is cancelled for extraordinary reasons.
- **Discussions** (organized by topic) are the primary Q&A forum. Email only if Discussions can't answer.
- Questions already answered in FAQ, or emailed instead of posted, get **lower priority**. Emails to other addresses go unanswered.
- **Code of honour** applies: https://www.kth.se/en/eecs/utbildning/hederskodex
- Generative AI tools page: `L01 - Introduction and practicalities/`
- Disability support: see the *Disability* page on Canvas.

---

## 7. Your status tracker

| Item | Deadline | Status |
|---|---|---|
| Ethics essay (RAP1) | 9 Nov | ❌ not submitted (deadline passed) |
| Search assignment + journal | 23 Nov 19:00 | ⬜ |
| Classroom quiz Search | — | ✅ passed (3.0) |
| HMM assignment + journal | 30 Nov 19:00 | ⬜ |
| Classroom quiz HMM | TBA slots | ⬜ |
| RL assignment + journal | 7 Dec 19:00 | ⬜ |
| Classroom quiz RL | TBA slots | ⬜ |
| Canvas quizzes Q0–Q5 | 8 Jan 19:00 | ⬜ all |
| Oral exam | after 7 Dec | ⬜ book slot |

---

## 8. What's in the folder

```
DD2380_Artificial_Intelligence/
├── L01 - Introduction and practicalities/   Lecture 1a Intro, 1b Practicalities, GenAI tools page
├── L02 - AI and Society (ethics)/           Ethics lecture, Ethics Canvas, Hazards Table, Roboted, Robots in Society
├── L03-04 - Search and Games/               Search, Adversarial Search, Search Tutorial
├── L05 - Knowledge, reasoning, planning/    Logic and Planning
├── L06-07 - Probabilistic reasoning and HMMs/  Probabilistic Reasoning, HMMs, 3 HMM tutorials
└── Assignments/
    ├── DD2380_2026_Search_Assignment.pdf + skeleton (extracted)
    ├── DD2380 2026 HMM Assignment + fishingderby_hmm (extracted)
    └── hmm_c_N1000.in, hmm_c_N10000.in
```

**Not downloaded:** the Super Mario slides link points at another Canvas course (49134) with different enrolment.

---

## 9. Study approach that actually matches the grading

1. **Kattis first, journal second, but both are weekly work.** Getting Part 3 then writing the journal in one night is how people land B instead of A.
2. **Write the journal as you build.** Each design decision, each failed attempt, each result — that's the raw material for E vs D and B vs A distinctions.
3. **Keep a one-page "explain it out loud" summary per assignment.** That's your oral exam prep, and it's the difference between an A and a C cap.
4. **Do the Canvas quizzes the week they unlock.** They're 60% to pass with 5 attempts — cheap insurance, don't stack them into January.
5. **Book the on-campus quiz slots early.** 4 slots each, and the HMM/RL ones are still open.
