# Stage 2 — Classical Machine Learning

## What This Stage Covers

The mathematical heart of traditional ML. Every algorithm here is studied *from first principles* — you derive cost functions, understand why regularization works geometrically, and implement gradient descent from scratch before using sklearn.

| Topic | Key Math |
|-------|---------|
| Linear Regression | OLS, RSS minimization, normal equations, R² |
| Logistic Regression | Bernoulli MLE → binary cross-entropy loss, sigmoid, decision boundary |
| Regularization (L1/L2) | Ridge as Lagrangian constrained optimization; Lasso and sparse solutions |
| Support Vector Machines | Margin maximization, Lagrangian duality, kernel trick |
| Decision Trees | Information gain, Gini impurity, CART algorithm |
| Ensembles | Bagging (variance reduction), Random Forests, Boosting (gradient boosting derivation) |
| k-Nearest Neighbors | Distance metrics, curse of dimensionality |
| Clustering | k-means (EM-style update), GMMs (full EM algorithm), DBSCAN |
| Dimensionality Reduction | PCA via SVD (derived), t-SNE (intuition) |
| Model Selection | CV, bootstrap, bias-variance tradeoff |

---

## Learning Goals

By the end of Stage 2, you should be able to:

- ✅ Derive the MSE cost function from MLE for linear regression
- ✅ Derive the logistic regression log-likelihood and its gradient
- ✅ Explain ridge/lasso regularization as constrained optimization (Lagrangian form)
- ✅ Implement gradient descent in NumPy (no sklearn) for regression
- ✅ Explain the SVM margin maximization as a quadratic program
- ✅ Derive gradient boosting as functional gradient descent
- ✅ Derive PCA from SVD and implement it in NumPy
- ✅ Explain the EM algorithm and its application to GMMs

---

## Time Estimate

| Resource | Hours |
|----------|-------|
| ISLR 2nd Ed. + Stanford edX (primary) | ~55–120 hrs |
| Andrew Ng ML Specialization (supplementary 1) | ~60–100 hrs |
| StatQuest ML playlists (supplementary 2) | ~30–50 hrs |
| **Total** | **~145–270 hrs** |

> **Realistic pace:** 15–20 hrs/week → **2–4 months**

---

## Study Order

```
Months 1–4:  ISLR 2nd Ed. + Stanford edX (PRIMARY) — read chapter, watch lectures, do labs
Parallel:    Andrew Ng ML Specialization (SUPP 1) — watch alongside ISLR for intuition
Throughout:  StatQuest ML playlist (SUPP 2) — watch relevant videos before/after each chapter
Reference:   CS229 lecture notes for derivations that need more depth
Reference:   ESL PDF for advanced deep-dives
```

---

## Critical Math-Rigor Checkpoints (Don't Skip These)

1. **ISLR Ch. 3** — Work through ALL exercises (derive RSS, R², ridge solutions by hand)
2. **ISLR Ch. 4, Section 4.4** — Logistic regression via MLE; don't skip
3. **ISLR Ch. 6** — Ridge/Lasso as Lagrangian constrained optimization
4. **ISLR Ch. 9** — SVM margin maximization derivation; supplement with StatQuest SVM playlist
5. **ISLR Ch. 12** — PCA via SVD is fully derived; pair with StatQuest "PCA Step-by-Step"
6. **Andrew Ng Course 1, Week 2** — Manually implement gradient descent in NumPy (no sklearn)

---

## Notes

- For GMMs specifically: ISLR touches on this lightly (Ch. 12). Supplement with CS229 lecture notes on EM algorithm: http://cs229.stanford.edu/notes/cs229-notes8.pdf (always public)
- ESL (Elements of Statistical Learning) is a reference, not a course. Keep the free PDF bookmarked for when ISLR's treatment feels insufficient.
