# Stage 0 — Sources

## 🏆 Primary: Linear Algebra

### [MIT OCW 18.06SC — Linear Algebra (Gilbert Strang)](https://ocw.mit.edu/courses/18-06sc-linear-algebra-fall-2011/)

- **Type:** Video course + problem sets + exams (Scholar version)
- **Cost:** Free
- **Math depth:** ⭐⭐⭐⭐⭐ — Derives proofs, covers SVD, eigendecomposition, and matrix decompositions from first principles
- **Why this one:** The gold standard for linear algebra — universally cited on r/MachineLearning, r/learnmachinelearning, and Hacker News as the #1 recommendation. The Scholar version adds recitation videos and worked solutions. Covers every ML-critical topic: vectors, matrix operations, orthogonality, eigenvalues/eigenvectors, positive definite matrices, and SVD in full. Strang's pedagogy is famously rigorous yet intuitive. **Rejected alternative:** Khan Academy — too shallow (skips proofs, SVD not covered at ML depth) and lacks the problem sets that build real skill. **Note:** Prof. Strang retired May 2023; videos are permanently archived.
- **Prerequisite:** High school algebra (no calculus required for most of the course)
- **Est. time:** 80–120 hrs (full); 50–60 hrs for ML-targeted subset through SVD
- **Companion video:** [3Blue1Brown Essence of Linear Algebra](https://youtube.com/playlist?list=PLZHQObOWTQDPD3MizzM2xVFitgF8hE_ab) — watch this FIRST (3–4 hrs) to build visual intuition before starting 18.06

---

### [MIT OCW 18.065 — Matrix Methods in Data Analysis, Signal Processing, and ML](https://ocw.mit.edu/courses/18-065-matrix-methods-in-data-analysis-signal-processing-and-machine-learning-spring-2018/)

- **Type:** Video lectures + problem sets (archived Spring 2018)
- **Cost:** Free
- **Math depth:** ⭐⭐⭐⭐⭐ — Applied ML focus; derives SVD for PCA, analyzes gradient descent convergence, covers statistical learning
- **Why this one:** The missing bridge between 18.06's abstract linear algebra and real ML algorithms. Covers SVD applied to low-rank approximation and PCA, gradient descent analysis, backpropagation, and statistical applications — directly relevant to every subsequent stage. Companion book: *Linear Algebra and Learning from Data* (Strang, 2019). **Note:** Take AFTER completing 18.06.
- **Prerequisite:** MIT 18.06 (Stage 0 Phase 2)
- **Est. time:** 50–60 hrs

---

## 🏆 Primary: Calculus

### [3Blue1Brown — Essence of Calculus](https://youtube.com/playlist?list=PLZHQObOWTQDMsr9K-rj53DwVRMYO3t5Yr) + [MIT Matrix Calculus for ML and Beyond (IAP 2023)](https://ocw.mit.edu/courses/18-s096-matrix-calculus-for-machine-learning-and-beyond-january-iap-2023/)

- **Type:** Video series (3B1B) + IAP course with lecture notes and videos (MIT)
- **Cost:** Free
- **Math depth:** ⭐⭐⭐☆☆ (3B1B intuition) + ⭐⭐⭐⭐⭐ (MIT Matrix Calculus depth)
- **Why this one:** MIT 18.01/18.02 (120–160 hrs) covers calculus topics mostly irrelevant to ML (surface integrals, vector fields, etc.). The MIT Matrix Calculus for ML IAP course delivers exactly what ML needs — matrix derivatives, Jacobians, Hessians, and the chain rule in matrix notation — in ~20 hrs. 3Blue1Brown provides the intuition layer (~4 hrs). Together they deliver 90% of the ML calculus value in ~25% of the time of the full 18.01/18.02 path. **Supplementary:** [Parr & Howard "The Matrix Calculus You Need for Deep Learning"](https://arxiv.org/abs/1802.01528) (free arXiv paper, ~40 pages) — concise reference for backprop math.
- **Prerequisite:** 3Blue1Brown LA (watch first); MIT Matrix Calculus requires some 18.06 familiarity
- **Est. time:** 3B1B ~4 hrs + MIT IAP ~15–20 hrs = **~20–25 hrs total**

---

## 🏆 Primary: Probability & Statistics

### [StatQuest with Josh Starmer](https://www.youtube.com/@statquest) + [Harvard STAT110 (Joe Blitzstein)](https://youtube.com/playlist?list=PL2SOU6wwxB0uwwH80KTQ6ht66KWxbzTIo)

**StatQuest:**
- **Type:** YouTube video series (short, 5–20 min per topic)
- **Cost:** Free
- **Math depth:** ⭐⭐⭐☆☆ — Intuitive but correct; covers MLE, MAP, Bayes, distributions with visual worked examples
- **Est. time:** ~20–25 hrs (Statistics Fundamentals + ML-relevant playlists)
- **Subscriber count as of July 2026:** ~1.66M — consistently cited as the #1 stats resource for ML practitioners

**Harvard STAT110:**
- **Type:** Video lectures (~34 × 75 min) + free textbook (Blitzstein & Hwang)
- **Cost:** Free (YouTube + free PDF); edX version has interactive problems (optional)
- **Math depth:** ⭐⭐⭐⭐☆ — Full probability derivations; "story proofs" style; covers conditional probability, distributions, MLE, CLT, Markov chains
- **Textbook:** https://projects.iq.harvard.edu/stat110/home (free)
- **Est. time:** ~80–100 hrs (full); focus on Lectures 1–20 for core ML probability (~40 hrs)

- **Why this combination:** StatQuest makes MLE, MAP, and Bayes *accessible* in ML context; STAT110 provides the mathematical depth needed to read papers. **Rejected alternative:** MIT 6.041 — equally rigorous but requires multivariable calculus as a hard prereq and is harder to follow without a TA; better for the PhD track. STAT110 is more accessible while mathematically complete.

---

## 🔗 Unifying Reference

### [Mathematics for Machine Learning — Deisenroth, Faisal, Ong](https://mml-book.github.io/)

- **Type:** Textbook (free PDF)
- **Cost:** Free (PDF); print ~$50
- **Math depth:** ⭐⭐⭐⭐☆ — University-level, ML-targeted; covers all four pillars with ML-specific examples
- **Why this one:** The most ML-targeted math textbook available for free. Part I covers: Linear Algebra, Analytic Geometry, Matrix Decompositions (SVD in full), Vector Calculus (Jacobians, Hessians, backpropagation), Probability & Distributions, and Continuous Optimization (convexity, gradient descent, Lagrange multipliers/KKT). Part II applies math directly to Linear Regression, PCA, GMMs, and SVMs. **Chapter 7 (Continuous Optimization) is the primary source for optimization topics** — no standalone free course covers convexity + gradient descent + Lagrange multipliers as concisely.
- **Usage mode:** Read alongside primary sources, not as a standalone course. When 18.06 covers eigenvalues → open MML Chapter 4 to see SVD applied to PCA.
- **Prerequisite:** Some prior exposure to calculus and linear algebra recommended
- **Est. time:** ~40–60 hrs (Part I targeted); ~120–150 hrs (full book)

---

## ❌ Rejected Candidates

| Resource | Reason Rejected |
|----------|----------------|
| **Khan Academy (primary)** | Too shallow — skips proofs, SVD not covered at ML depth, Jacobians missing. Best as a gap-filler for high school review only |
| **MIT 18.01/18.02 (primary calculus)** | 120–160 hrs for content with ~30% ML relevance. The MIT Matrix Calculus IAP delivers ML calculus in ~20 hrs |
| **MIT 6.041 (primary probability)** | Requires multivariable calculus as hard prereq; harder and longer than STAT110 with less pedagogical accessibility. Excellent for PhD track — keep as optional reference |
| **DeepLearning.AI Math for ML Specialization (Coursera)** | Paid (~$50/month); lower depth than 18.06 + MML combo; some reviewers flag non-standard explanations in probability module. Good, but not best. |

---

## 📋 Key Playlists & Direct Links

| Resource | Direct Link |
|----------|------------|
| 3B1B Essence of Linear Algebra | [YouTube Playlist](https://youtube.com/playlist?list=PLZHQObOWTQDPD3MizzM2xVFitgF8hE_ab) |
| 3B1B Essence of Calculus | [YouTube Playlist](https://youtube.com/playlist?list=PLZHQObOWTQDMsr9K-rj53DwVRMYO3t5Yr) |
| MIT 18.06SC (Scholar version) | [OCW Course](https://ocw.mit.edu/courses/18-06sc-linear-algebra-fall-2011/) |
| MIT 18.065 | [OCW Course](https://ocw.mit.edu/courses/18-065-matrix-methods-in-data-analysis-signal-processing-and-machine-learning-spring-2018/) |
| MIT Matrix Calculus IAP 2023 | [OCW Course](https://ocw.mit.edu/courses/18-s096-matrix-calculus-for-machine-learning-and-beyond-january-iap-2023/) |
| StatQuest YouTube | [Channel](https://www.youtube.com/@statquest) |
| StatQuest Video Index | [statquest.org](https://statquest.org/video-index/) |
| Harvard STAT110 YouTube | [Playlist](https://youtube.com/playlist?list=PL2SOU6wwxB0uwwH80KTQ6ht66KWxbzTIo) |
| STAT110 Free Textbook | [harvard.edu](https://projects.iq.harvard.edu/stat110/home) |
| MML Book (free PDF) | [mml-book.github.io](https://mml-book.github.io/) |
| Parr & Howard Matrix Calculus paper | [arXiv](https://arxiv.org/abs/1802.01528) |
| CS229 Math Notes (reference) | [stanford.edu](http://cs229.stanford.edu/section/cs229-linalg.pdf) |
