# Stage 2 — Sources

## 🏆 Primary

### [An Introduction to Statistical Learning (ISLR 2nd Ed.) + Stanford edX](https://www.statlearning.com)

- **Type:** Textbook + video course (Stanford edX, author-taught)
- **Cost:** Free PDF (official download at statlearning.com); edX audit is free; verified certificate ~$149
- **Math depth:** ⭐⭐⭐⭐☆ — Derives cost functions, logistic regression from MLE, ridge/lasso as constrained optimization, SVM margin maximization via Lagrangian duality, PCA via SVD. Rigorous without being needlessly opaque — shows math alongside geometric intuition
- **Why this one:** ISLR is the only resource in the candidate list that simultaneously: (1) derives things from first principles — logistic regression cost via MLE, lasso/ridge as Lagrangian, PCA via SVD, SVM via Lagrangian duality; (2) hits ALL requested topics; (3) is fully free; (4) has a Python edition (ISLP, 2023 — no R required); (5) has a structured author-taught Stanford video course. The 2nd edition (2021) added deep learning, survival analysis, and multiple testing. The Python edition (ISLP) was released in 2023. **Crucially, ISLR achieves math depth that Andrew Ng's course does not** — it formally writes out the optimization objective for ridge regression, proves why PCA eigendecomposition equals SVD, and shows the full VC dimension intuition for SVMs.
- **Prerequisite:** Basic linear algebra and introductory statistics (Stage 0); Python (Stage 1)
- **Est. time:** ~55–66 hrs (11 weeks × 5–6 hrs/week on edX); full textbook self-study ~80–120 hrs
- **Links:**
  - Free PDF: https://www.statlearning.com
  - ISLP (Python edition, also free PDF): https://www.statlearning.com
  - Stanford edX course: https://www.edx.org/learn/python/stanford-university-statistical-learning-with-python
  - CS229 EM notes (supplement for GMMs): http://cs229.stanford.edu/notes/cs229-notes8.pdf

---

## 📌 Supplementary 1

### [Andrew Ng — Machine Learning Specialization (Coursera, 2022)](https://www.coursera.org/specializations/machine-learning-introduction)

- **Type:** 3-course specialization; video lectures + Jupyter labs + quizzes (self-paced)
- **Cost:** ~$49–79/month Coursera subscription (typically 2–3 months = ~$100–237). **Audit for free** (no graded assignments). Financial aid available.
- **Math depth:** ⭐⭐⭐☆☆ — Derives logistic regression cost from MLE intuition; shows gradient descent update rules; covers L1/L2 regularization effect on weights. Does NOT do full formal proofs or matrix-calculus derivations. "Intuition-first" philosophy.
- **Why this one:** The 2022 version is a complete rewrite in Python (numpy/sklearn/tensorflow) and is genuinely math-rigorous by popular standards — you implement gradient descent from scratch in NumPy, manually code regularized logistic regression, and build neural networks layer by layer. **Use BEFORE or ALONGSIDE ISLR** — Ng's ability to build intuition is unmatched; after his explanation of gradient descent, ISLR's math clicks immediately. Course 3 covers clustering (k-means), anomaly detection, and recommender systems — topics ISLR gives less attention to, making it genuinely complementary.
- **Prerequisite:** None formally required (ISLR's Stage 0 prereqs make it more accessible)
- **Est. time:** ~60–100 hours
- **deeplearning.ai page:** https://www.deeplearning.ai/courses/machine-learning-specialization/

---

## 📌 Supplementary 2

### [StatQuest with Josh Starmer — ML Playlists](https://www.youtube.com/@statquest)

- **Type:** YouTube video series (short, self-contained, 10–30 min per topic)
- **Cost:** Free (100%). Optional paid "Study Guides" on statquest.org (~$9 each)
- **Math depth:** ⭐⭐⭐⭐☆ — Shows the math for each topic visually. Does not shy away from formulas. Covers gradient boosting derivation, logistic regression log-likelihood, PCA step-by-step via SVD, SVM margin math. Not proof-heavy but fully transparent.
- **Why this one:** StatQuest is the perfect complement to ISLR — where ISLR presents math on the page, StatQuest animates it visually. When a chapter in ISLR feels unclear, a StatQuest video on the same topic almost always unlocks it. Its gradient boosting and PCA via SVD videos are arguably the single best treatments of those topics available for free anywhere.
- **Prerequisite:** None — scales from basics to advanced
- **Est. time:** ~30–50 hours to cover all classical ML topics
- **Key playlists:**
  - [Gradient Boosting series](https://www.youtube.com/watch?v=3CC4N4z3GJc)
  - [PCA Step-by-Step](https://www.youtube.com/watch?v=FgakZw6K1QQ)
  - [Logistic Regression series](https://www.youtube.com/watch?v=yIYKR4sgzI8)
  - [Random Forests series](https://www.youtube.com/watch?v=J4Wdy0Wc_xQ)
  - [SVM playlist](https://www.youtube.com/watch?v=efR1C6CvhmE)

---

## ❌ Rejected Candidates

| Resource | Reason Rejected |
|----------|----------------|
| **CS229 Stanford (primary)** | Exceptional (gold standard for graduate rigor) but violates practical constraints: steep prereqs (solid linear algebra + calc + probability BEFORE starting), 15–20 hrs/week for enrolled students, and most widely-referenced videos are 2018 vintage. Best used as a **reference** for specific derivations (lecture notes at cs229.stanford.edu are always free) |
| **ESL (Elements of Statistical Learning)** | Requires PhD-level mathematical maturity. Even the authors recommend reading ISLR first. Keep free PDF bookmarked for reference when ISLR is insufficient. [Free PDF](https://hastie.su.domains/ElemStatLearn/) |
| **fast.ai Practical Deep Learning** | The 2022/2023 version is heavily deep-learning focused with only cursory classical ML coverage. Its older "Introduction to ML for Coders" (2018) covers random forests in depth but uses outdated APIs. fast.ai's top-down philosophy is the opposite of what's needed for a math-rigorous Stage 2. **Correct use:** Stage 3 and beyond |

---

## 📋 ISLR Chapter Map (ML Topics)

| ISLR Chapter | Topics | Math Highlights |
|-------------|--------|----------------|
| Ch. 2 | Statistical Learning overview | Bias-variance tradeoff |
| Ch. 3 | Linear Regression | RSS, R², OLS normal equations |
| Ch. 4 | Classification | Logistic regression via MLE, LDA, QDA |
| Ch. 5 | Resampling | Cross-validation, bootstrap |
| Ch. 6 | Linear Model Selection | Ridge, Lasso (Lagrangian), elastic net |
| Ch. 7 | Moving Beyond Linearity | Polynomials, splines, GAMs |
| Ch. 8 | Tree-Based Methods | Bagging, random forests, boosting |
| Ch. 9 | SVMs | Maximal margin classifier, Lagrangian duality, kernels |
| Ch. 10 | Deep Learning | (intro — Stage 3 will go much deeper) |
| Ch. 12 | Unsupervised Learning | PCA via SVD, k-means, hierarchical clustering |
| Ch. 13 | Multiple Testing | FDR, Bonferroni |
