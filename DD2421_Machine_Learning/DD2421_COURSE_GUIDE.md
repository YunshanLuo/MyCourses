# DD2421 / FDD3431 HT26 — Machine Learning

> **Everything in the course, plus everything you owe it.**
> Snapshot: 2026-11-14 · Materials: `courses/DD2421_Machine_Learning/`
> Canvas: https://canvas.kth.se/courses/63976

---

## 1. At a glance

| | |
|---|---|
| **Course codes** | DD2421 / FDD3431 Machine Learning |
| **Credits** | 7.5 hp |
| **Examiner / course responsible** | Atsuto Maki |
| **Lecturers** | Atsuto Maki, André Pereira, Jörg Conradt |
| **Course assistant / Head of TAs** | Alexander Kozlov (akozlov@kth.se) |
| **Schedule** | https://www.kth.se/social/course/DD2421/calendar/ |
| **Textbook** | James, Witten, Hastie, Tibshirani — *An Introduction to Statistical Learning with Applications in Python* (Springer 2021), **free** at https://www.statlearning.com/ |
| **Registration questions** | service@eecs.kth.se (**not** the teachers) |
| **Status right now** | Lectures done · labs 1–3 past due · **written exam was 16 Oct** |

---

## 2. Recommended literature

**Primary**
- *An Introduction to Statistical Learning with Applications in Python* — James, Witten, Hastie, Tibshirani (Springer 2021) — https://www.statlearning.com/

**Additional**
- *Computer Vision: Models, Learning, and Inference* — Simon J.D. Prince — selected chapters — http://www.computervisionmodels.com/
- *Neural Networks — A Systematic Introduction* — Raul Rojas, ch. 3+4 and 6+7 — https://link.springer.com/book/10.1007/978-3-642-61068-4 (also in `99 - Misc/`)
- *The Elements of Statistical Learning* — Hastie, Tibshirani, Friedman — https://web.stanford.edu/~hastie/ElemStatLearn/

---

## 3. Lecture map

Lectures are **not recorded**. Slides are uploaded to Canvas in advance.

| # | Topic | Contents | Reading | Lecturer | Folder |
|---|---|---|---|---|---|
| 1 | Introduction | Course logistics; what is a "learning machine"; supervised vs unsupervised; nearest neighbour | ISL §2.1–2.2 | Maki, Pereira, Conradt | `L01` |
| 2 | Decision Trees | What/when are they useful; choosing questions; entropy; information gain; overfitting; extensions | ISL §8.1 | Maki | `L02` |
| 3 | Challenges in ML | Prediction errors; model complexity and overfitting; cross-validation; curse of dimensionality; bias–variance | ISL §2, 5.1, 6.4 | Maki | `L03` |
| 4 | Regression | Linear regression; RANSAC; regularisation (ridge, lasso); nearest-neighbour regression; parametric vs non-parametric | ISL §3.1, 3.2, 3.5, 6.2 | Maki | `L04` |
| 5 | Support Vector Machines | Hyperplane classification; incremental learning; structural risk minimisation; SVM; kernels; overlapping classes | see svm-tutorial.com | Conradt | `L05` |
| 6 | Artificial Neural Networks | Biological neuron; perceptron; single-neuron learning; multi-layer nets; backpropagation; practical tricks; recurrent/unsupervised/deep nets | Rojas ch. 3+4, 6+7 | Conradt | `L06` |
| 7 | Probabilistic Reasoning | Intro to probabilistic ML; probability foundations; common distributions; probabilistic classification | Prince Part I (ch. 2, 3, 5) | Pereira | `L07` |
| 8 | Probabilistic Learning | Probability estimation assumptions; MLE for regression; MLE for classification (continuous/discrete); Naïve Bayes; logistic regression | ISL ch. 4, Prince | Pereira | `L08` |
| 9 | Priors and Latent Variables | MAP estimate; Bayesian non-parametrics; model selection and Occam's razor; unsupervised learning; K-means; Expectation Maximisation | Prince 4.4.2, 7.1–7.4, 8.1, 9.1 | Pereira | `L09` |
| 10 | Ensemble Methods | Why combine classifiers; bagging; decision forests; boosting | ISL §8.2 | Maki | `L10` |
| 11 | Dimensionality Reduction | PCA; subspace concept; similarity measures; subspace methods; Fisher's criterion | ISL §12.2, 4.4 | Maki | `L11` |
| 12 | Three mini lectures + exam Q&A | Topics **beyond exam scope** | — | Maki, Pereira, Conradt | — |

**Exam scope: Lectures 1–11 only.**

Each lecture folder also has demo notebooks: `CLT_illustration-1.ipynb`, `Curse_demo-2.ipynb`, `Linear Bayes Regression-3.ipynb`, `GMM-2.ipynb`.

---

## 4. Everything you must do

### 4.1 Labs — 3, presented orally to a TA

| Lab | Topic | Due | Files |
|---|---|---|---|
| **Lab 1** | Decision Trees | 11 Sep 16:00 | `Assignments/dectrees.zip` |
| **Lab 2** | Support Vector Machines | 23 Sep 16:00 | `Assignments/svm-2018.pdf` |
| **Lab 3** | Bayes Classifiers and Boosting | 9 Oct 16:00 | `Assignments/Bayes+boosting.zip` |

**Labs are Pass/Fail and presented — there is no written report.**
- Book a 15-minute slot in Canvas Calendar (2 students per slot)
- **Be ready to present the whole lab in 10 minutes** — slides, or figures and numbers
- Order of presentation is decided by the TA; be prepared to present any part
- The **program code is not discussed** during review — use help sessions for that
- Have all results ready to support your conclusions

**Event types**
- **Lab review** — evaluation, 2h split into 15-min slots, bookable, on campus
- **Lab help** — 1h drop-in, no booking needed (recommended anyway), on campus or online per Calendar
- **Lab Q&A** — 1h split into 10-min slots (1 student), bookable, on **Zoom**

**Booking rules**
- One slot per lab report; don't book multiple unless rejected
- Put the **lab number in Comments**; don't put other students' names
- Each partner books their own time; try for the same slot, split if needed
- Book early — missing the deadline delays reporting and Ladok registration

### 4.2 Written examination

- **Scope: Lectures 1–11**
- Several questions; **~50% of full points needed to pass**
- **Aid allowed: only a calculator and a language dictionary.**
  No notes, no formula sheets, no prepared reference material.
- **You must register for the exam** to sit it — teachers cannot help with registration; contact your student office.
- *Plussning* (grade improvement) **is permitted at the re-exam**.

### 4.3 Lab environment setup

The course recommends Python 3.11 with `uv`:

```bash
uv venv --python 3.11.15
uv pip install --python .venv -r requirements-lab3.txt
uv run jupyter notebook lab3.ipynb
```

**Known Lab 3 errata** — in `labfuns.py` change:
```python
from sklearn.datasets.samples_generator import make_blobs   # old, broken
from sklearn.datasets import make_blobs                     # correct
```

`requirements-lab3.txt` is referenced on the Canvas setup page (not downloadable in the bulk sync).

---

## 5. Grade requirements — what "A" actually means

To reach a grade you must satisfy all criteria at that level **and all lower levels**.

### E — use terminology, solve standard problems
- Define and correctly use standard ML terms
- Use a k-nearest neighbour classifier
- Design and use decision trees
- Use probability theory to explain aspects of ML
- Use Bayesian classification on simple problems
- Use SVMs for linear classification

### D — do the calculations by hand, know the limits
- Calculate predictability of data using entropy
- Calculate optimal model parameters in a probabilistic framework from data points
- Explain overtraining and suggest methods to avoid it

### C — apply algorithms to novel problems
- Apply an appropriate regression algorithm to a novel problem
- Apply the Expectation Maximisation algorithm to a novel problem
- Describe how boosting works and when it can be used

### B — use the theory
- Use non-linear SVM for harder problems
- Analyse and reflect on ensemble methods in terms of bias–variance trade-off
- Define overfitting and model selection in Bayesian terms

### A — use and describe everything, extrapolate
- Use and describe all techniques with none or very few errors
- Extrapolate solutions to problems not covered in the lectures

*(Bullet points are examples, not exhaustive.)*

---

## 6. Course FAQs

- **Can we present the lab over Zoom?** No — everyone presents on site.
- **Are slides available?** Yes, uploaded under *Lectures* in advance.
- **Zoom Q&A?** Only the 10-minute Lab Q&A slots.
- **Registration questions** → service@eecs.kth.se, not the teachers.
- Generative AI policy: not specified for this course in Canvas — check the course memo or ask the instructor.

---

## 7. Your status tracker

| Item | Due | Status |
|---|---|---|
| Lab environment set up | — | ⬜ |
| Lab 1 (Decision Trees) | 11 Sep | ⬜ past due |
| Lab 2 (SVM) | 23 Sep | ⬜ past due |
| Lab 3 (Bayes + Boosting) | 9 Oct | ⬜ past due |
| Written exam | 16 Oct | ❌ |
| **Re-exam** | **TBA** | 🎯 if you need it — *plussning* allowed |

---

## 8. What's in the folder

```
DD2421_Machine_Learning/
├── L01/  Lecture 1 - Introduction.pdf, Lecture 1 - Course intro (HT26).pdf
├── L02/  Lecture 2 - Decision Trees (Autumn 2026).pdf, (4-up).pdf
├── L03/  Lecture 3 - Challenges in ML.pdf
├── L04/  Lecture 4 - Regression.pdf
├── L05/  Lecture 5 - Support Vector Machines.pdf
├── L06/  Lecture 6 - Artificial Neural Networks.pdf
├── L07/  Lecture 7 - Probabilistic Reasoning.pdf + (handout).pdf
├── L08/  Lecture 8 - Probabilistic Learning.pdf
├── L09/  Lecture 9 - Priors and Latent Variables.pdf
├── L10/  Lecture 10 - Ensemble Methods.pdf
├── L11/  Lecture 11 - Dimensionality Reduction.pdf
├── Assignments/  dectrees.zip, svm-2018.pdf, Bayes+boosting.zip, ML lab requirements-lab3.txt
├── Exam/  5 past exams + solutions/commentaries (HT2025, VT2026, VT2025, HT2024, 2026-03-11)
└── 99 - Misc/  Rojas Neural Networks book, demo notebooks (CLT, Curse, GMM, Linear Bayes)
```

The `Exam/` folder is the most valuable part for re-exam prep — those commentaries tell you what the examiner actually rewards.

---

## 9. Exam-prep approach

1. **Aid is calculator + dictionary only.** Everything must be memorised or derivable. Practise deriving by hand: entropy, information gain, MLE, MAP, SVM margins.
2. **Work the `Exam/` papers in exam conditions**, then read the commentaries. The gap between your answer and the commentary is your study list.
3. **The grade levels are the exam blueprint.** Each bullet under E/D/C/B/A maps to a question type. If you can do every D-level calculation cleanly, you're safe at D; C requires applying to novel setups.
4. **Know the algorithms you can be asked to compute**: decision tree splits, k-NN, Naïve Bayes, logistic regression MLE, EM for GMMs, PCA, boosting rounds.
5. **Bias–variance shows up at every level** — as an explanation (E), an analysis (B), and in ensemble context (B). Don't skip it.
6. Lab 3's errata bit is a classic time sink — fix `labfuns.py` before you start if you're redoing labs.
