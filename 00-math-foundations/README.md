# Stage 0 — Math Foundations

## What This Stage Covers

Before touching a single line of ML code, you need fluency in the four mathematical pillars that every algorithm in this roadmap is built on:

| Pillar | Why It Matters |
|--------|---------------|
| **Linear Algebra** | ML models *are* linear algebra — weights are matrices, activations are vectors, SVD underlies PCA and recommendation systems |
| **Calculus** | Training is optimization — you need derivatives, chain rule, Jacobians, and Hessians to understand backpropagation and gradient descent |
| **Probability & Statistics** | Uncertainty is everywhere — MLE derives cost functions, Bayes grounds probabilistic models, hypothesis testing validates results |
| **Optimization** | Every model trains by minimizing a loss — convexity theory tells you *when* a minimum exists; Lagrange multipliers explain SVMs and regularization |

---

## Learning Goals

By the end of Stage 0, you should be able to:

- ✅ Compute matrix multiplications, inverses, and determinants by hand
- ✅ Explain what eigenvalues/eigenvectors represent geometrically
- ✅ Derive SVD and explain why PCA is a special case of it
- ✅ Apply the chain rule to multivariate composite functions (Jacobian)
- ✅ Compute the gradient of a loss function with respect to weight matrices
- ✅ State and apply Bayes' Theorem in a probabilistic ML context
- ✅ Derive the MLE objective for linear regression (proves MSE loss)
- ✅ Explain convexity and why it guarantees a global minimum
- ✅ Set up a Lagrange multiplier problem and solve the KKT conditions

---

## Time Estimate

| Phase | Content | Hours |
|-------|---------|-------|
| Phase 1 — Intuition | 3Blue1Brown LA + Calculus + StatQuest fundamentals | ~20–25 hrs |
| Phase 2 — Core Courses | MIT 18.06SC + STAT110 + MIT Matrix Calculus | ~150–180 hrs |
| Phase 3 — Integration | MML Book Part I + MIT 18.065 | ~80–100 hrs |
| **Total** | | **~250–305 hrs** |

> **Realistic pace:** 15–20 hrs/week → **3–5 months**

---

## Study Order

```
Week 1–2:    3Blue1Brown — Essence of Linear Algebra (all 15 chapters)
Week 2–3:    3Blue1Brown — Essence of Calculus (all 12 chapters)
Week 3–4:    StatQuest — Statistics Fundamentals playlist (top 20 videos)
Week 4–16:   MIT 18.06SC (primary linear algebra — work through SVD)
Week 4–16:   MML Book Part I (read alongside 18.06 as ML-context companion)
Week 8–20:   Harvard STAT110 (probability depth — Bayes, distributions, MLE)
Week 14–18:  MIT Matrix Calculus for ML (IAP 2023 — derivatives in matrix form)
Week 18–22:  MIT 18.065 (bridge: linear algebra → ML algorithms)
```

---

## Notes

- **Do not skip Phase 1.** The 3Blue1Brown intuition warm-up makes everything in Phase 2 click faster. It takes only ~15 hours.
- **MML Book Chapter 7** (Continuous Optimization) is your primary source for convexity, gradient descent, and Lagrange multipliers — no standalone course covers these as efficiently.
- **StatQuest** handles intuition; **STAT110** handles rigor — they are complementary, not redundant.
- **MIT 18.01/18.02** are NOT recommended as primary calculus — too broad for ML needs (120–160 hrs for content that has ~30% ML relevance). The MIT Matrix Calculus for ML IAP delivers 90% of the value in ~20 hrs.
