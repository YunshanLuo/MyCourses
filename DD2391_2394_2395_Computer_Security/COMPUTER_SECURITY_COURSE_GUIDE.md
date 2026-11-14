# DD2391 / DD2394 / DD2395 HT26 — Computer Security

> **Everything in the course, plus everything you owe it.**
> Snapshot: 2026-11-14 · Materials: `courses/DD2391_2394_2395_Computer_Security/`
> Canvas: https://canvas.kth.se/courses/64038

---

## 1. At a glance

| | |
|---|---|
| **Course codes** | DD2395 Computer Security · DD2391 Cybersecurity Overview · DD2394 Cybersecurity Project |
| **Examiner DD2395/DD2391** | Musard Balliu (musard@kth.se) |
| **Examiner DD2394** | Roberto Guanciale (robertog@kth.se) |
| **Teachers** | Musard Balliu, Sonja Buchegger (buc@kth.se), Roberto Guanciale |
| **Course email** | security-dd239x@kth.se |
| **Lab queue** | https://queue.csc.kth.se/Queue/Dasak |
| **Schedule** | https://www.kth.se/social/course/DD2395/calendar/ |
| **Textbook** | **None.** Handouts, papers and distributed material. Recommended: Anderson *Security Engineering* 3rd ed.; Gollmann *Computer Security* |
| **Status right now** | All 14 lectures done · written exam was **19 Oct** · labs/exercises due **30 Oct** · re-exam **16 Dec** |

**Which course are you in?** They share lectures but differ in what's mandatory:

| | DD2395 | DD2391 | DD2394 |
|---|---|---|---|
| Labs G/O/Z + exercises | ✅ | ✅ | ❌ |
| Lab W (web) | ✅ | ✅ | ❌ |
| Seminar | ✅ | ✅ (with project) | ❌ |
| Project | ❌ | ✅ | ✅ (only activity) |
| Written exam | ✅ | ✅ | ❌ |
| Final grade | A–F | A–F | Pass/Fail |

---

## 2. Lecture schedule & reading (actual 2026 dates — all completed)

Lectures 1–14 ran 27 Aug – 6 Oct. In-person, no recordings (some may be flipped classroom).

| Date | Topic | Preparation / reading | Folder |
|---|---|---|---|
| 27 Aug 15:00 | Course overview, intro to computer security | Schneider *Intro to cybersecurity*; Saltzer & Schroeder *Security principles* §1 | `L01` |
| 28 Aug 10:00 | Cryptography 101 | Wagner et al. Cryptography ch. 5, 6 | `L02` |
| 31 Aug 09:00 | Roberto: project task (DD2394/DD2391 only) | — | — |
| 31 Aug 13:00 | Cryptography 101 (cont.) | Cryptography ch. 7, 8, 9, 11, 12 | `L03` |
| 1 Sep 08:00 | Authentication and Authorization | Schneider §5.1, §7.1 (excl. 7.1.3), §7.2, §7.4, §8.1; Wagner ch. 14 | `L04` |
| 7 Sep 15:00 | Cryptography 2 | Interactive AES; Cryptography ch. 6, 10, 11 | `L05` |
| 8 Sep 08:00 | Web Application Security | Web Security ch. 17–22 | `L06` |
| 15 Sep 10:00 | Security protocols | TLS ch. 31 + lecture notes | `L07` |
| *prereq* | **Malware material** (watch before next 4 lectures) | Malware ch. 38 + videos + Stuxnet video | — |
| 15 Sep 15:00 | DoS vulnerabilities, firewalls, IDS | `r.zip` + lecture notes | `L08` |
| 21 Sep 08:00 | Memory safety | Memory safety ch. 2, 3 + Super Mario code injection | `L09` |
| 22 Sep 10:00 | Side channels | AES example + Schneider ch. 13 | `L10` |
| 28 Sep 10:00 | System security | Memory safety ch. 4 + Schneider ch. 10 | `L11` |
| 28 Sep 13:00 | Spectre and HW security | Spectre paper | `L12` |
| 5 Oct 10:00 | Social engineering + exam prep | — | `L13` |
| 6 Oct 10:00 | Exam preparation and course wrap-up | — | `L14` |

**Exams:** written exam 19 Oct 14:00–18:00 · **written re-exam 16 Dec 14:00–18:00**

---

## 3. Everything you must do

### 3.1 Labs — 3 mandatory + 1 optional

All graded **Pass/Fail**. You must pass all to pass the LAB part.

| Lab | What | Format | Merit points |
|---|---|---|---|
| **Lab G** — Secure email with GPG | Cryptography in practice | Individual, auto-graded | — |
| **Lab W** — Web application security | Exploit classic web attacks, reason about countermeasures | **Groups of 3**, requires TA presentation in pre-scheduled session | +1 for extra tasks |
| **Lab O** — Buffer overflow | Memory-unsafe exploitation, overflows and overreads | Individual, auto-graded, in provided container | +1 for extra tasks |
| **Lab Z** — Zip Bomb | DoS via malicious input | Individual, auto-graded, **optional** | +1 |

Lab O / Z / exercises all run in the **provided container** (Container method or VM method per the setup instructions).

### 3.2 Exercises — mandatory, auto-graded Pass/Fail

| Exercise | Topic |
|---|---|
| (In)secure hash function | Find a collision in a non-collision-resistant hash |
| Malware | Write a signature scanner detecting specific encrypting malware |
| Denial of Service | Build a filter detecting DoS-inducing inputs |
| Side channels | Attack a 2-round Feistel cipher via simulated direct-cache timing |

### 3.3 Seminar (DD2395 and DD2391 only)

- **Groups of 3**
- Deep-dive into one security topic: literature research + **live in-person presentation** in front of other groups
- Must also actively ask and answer questions
- Written component uploaded to Canvas
- Pass/Fail; required to pass LAB

### 3.4 Project (DD2391 and DD2394 only)

- **Groups of 4**
- Apply security knowledge to a concrete scenario/system: systems analysis, design, development, assessment
- **Presentation at a pre-scheduled session**
- Pass/Fail

### 3.5 Written exam (DD2395 and DD2391)

- Graded **A–F**
- Fx → can complement with an **oral discussion** to earn E
- **Grade improvement (*plussning*) is NOT allowed** for these courses
- Scope and structure "similar to exams and re-exams 2024/2025 and 2023/2024"
- Past exams + solutions available (2025/26 back to 2010) — see *Past Exams* page

---

## 4. Grading rules

**LAB:** Pass/Fail. Only reported once you've passed all mandatory lab activities, exercises and the seminar (+ project for DD2391/DD2394).

**Merit points:** labs allow a total of **3**. Needed only to raise the top end.

**DD2395 and DD2391 final grade:**

| Written exam grade | Merit points | Final grade |
|---|---|---|
| C or lower | any | **Same as exam** |
| A or B | 1 | **B** |
| A | 2 or 3 | **A** |

(All assuming LAB and, where relevant, Project are passed.)

**DD2394:** Pass/Fail, matching the project grade.

> So: merit points only matter if you're aiming for B or A. Everything else is exam-driven.

---

## 5. Course rules

- **Mandatory activities** (labs, exercises, seminar, project) must all be passed.
- **In person**: no remote participation, no lecture recordings. Pre-sentations (lab, seminar, project) require all group members present.
- **Questions:** check the relevant discussion thread → post there → lab session in person → `security-dd239x@kth.se` only in extreme cases.
- **Do NOT** message teachers via Canvas inbox (not checked) or email individuals directly.
- **Anonymous feedback:** via course representatives (Youssef Abdelrahman, Antoine Quint, Tim Solfronk).
- **Funka:** musard@kth.se with subject `[funka] <rest>`.
- **Code of honour:** https://www.kth.se/en/eecs/utbildning/hederskodex — cheating includes exchanging solutions between groups, misstating group contributions, and not citing sources.
- **AI tools:** the course has an explicit policy page — read it before using any.

---

## 6. Your status tracker

| Item | Due | Status |
|---|---|---|
| Lecture 1–14 | Aug–Oct | ✅ done |
| Lab G (GPG) | 30 Oct 17:00 | ⬜ past due |
| Lab W (Web) | 2 Oct 08:00 | ⬜ past due |
| Lab O (Overflow) | 30 Oct 17:00 | ⬜ past due |
| Lab Z (Zip Bomb, optional) | 30 Oct 17:00 | ⬜ past due |
| 4 exercises | 30 Oct 17:00 | ⬜ past due |
| Seminar | 9 Oct 13:00 | ⬜ past due |
| Cybersecurity Project | 20 Oct 21:30 | ⬜ past due |
| Written exam | 19 Oct | ❌ missed / not passed |
| **Written re-exam** | **16 Dec 14:00–18:00** | 🎯 **next action** |

**If you're sitting the 16 Dec re-exam**, the labs/exercises/seminar still need to be completed — the LAB component gates the final grade. Check the FAQ section "I took the course the previous years but did not complete all activities" for how prior-year work carries over.

---

## 7. What's in the folder

```
DD2391_2394_2395_Computer_Security/
├── L01 - Course overview and intro/       Lecture1.pdf, chptr.Intro.pdf, protection_information.pdf
├── L02 - Cryptography 101/                Lecture2.pdf
├── L03 - Cryptography 101 (cont.)/        Lecture3.pdf
├── L04 - Authentication and Authorization/ Lecture4.pdf, chptr.AuthPeople, chptr.DAC, chptr.MAC
├── L05 - Cryptography 2/                  Lecture5.pdf
├── L06 - Web Application Security/        Lecture6.pdf
├── L07 - Security protocols/              Computer Security protocols.pdf, notes-protocols.pdf, Protocols Updated.pdf
├── L08 - DoS, firewalls and IDS/          Computer Security DOS - FW.pdf, notes-dos.pdf, r.zip
├── L09 - Memory safety/                   Memory Safety.pdf, notes-memorysafety.pdf
├── L10 - Side channels/                   Side channels.pdf, notes-sidechannels.pdf
├── L11 - System security/                 SystemSec.pdf, notes-system-sec.pdf
├── L12 - Spectre and HW security/         Spectre.pdf, notes-spectre.pdf
├── L13 - Social engineering/              dasak26soceng-1.pdf
├── L14 - Exam preparation and wrap-up/    Lecture 14 slides, exam-problems-with-solutions-19Oct2026.pdf
└── Labs and Assignments/                  dasakLabG.pdf, dasakLabW.pdf, buc.pub, coursekey.pub, Crypto.drawio.png
```

**Not downloaded:** the Super Mario slides (hosted in Canvas course 49134, different enrolment).

Past exams live on the Canvas *Past Exams* page rather than the Files tab — worth pulling manually when you start re-exam prep.

---

## 8. Re-exam approach (16 Dec)

1. **Start from `L14 - Exam preparation and wrap-up/`** — the exam problems with solutions posted 19 Oct 2026 are the closest signal you'll get.
2. **Work backwards through the topics** in reverse lecture order; exam questions cluster around protocols, memory safety, side channels, and system security.
3. **Lecture notes PDFs matter as much as the slides** — each lecture has a `notes-*.pdf` companion that's tighter than the slides. Read those first for revision, use slides for depth.
4. **Lab work is not optional.** Check whether your prior labs count; if not, Lab G (individual, auto-graded, GPG) and the 4 exercises are the fastest path to a passing LAB.
5. **No *plussning*** — but an Fx can become an E through the oral discussion. Worth taking if you land on the boundary.
