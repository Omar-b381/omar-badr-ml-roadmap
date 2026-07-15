# 🧠 Omar Ahmed Badr — Math-First Machine Learning Roadmap

> **A mathematically rigorous, curated roadmap from first principles to production ML.**
> Not a "just call `.fit()`" tutorial list. Every stage derives concepts from the ground up.

---

## 📌 How to Use This Repo

1. **Follow stages in order** — each stage lists explicit prerequisites
2. **One primary source per stage** — curated, not exhaustive
3. **Track your progress** using `progress.md` files in each stage folder and [`PROGRESS.md`](PROGRESS.md) for the global view
4. **Free-first** — all primary sources are free; paid sources are only recommended where they add specific, irreplaceable value

---

## 🗺️ Stage Index

| # | Stage | Focus | Primary Source | Cost | Approx. Hours | Status |
|---|-------|-------|----------------|------|---------------|--------|
| 0 | [Math Foundations](00-math-foundations/) | Linear Algebra, Calculus, Probability, Optimization | MIT OCW 18.06 + StatQuest + MML Book | Free | ~150–200 hrs | ⬜ Not Started |
| 1 | [Programming & Data Tooling](01-programming-tools/) | Python, NumPy, Pandas, Matplotlib, Jupyter | CS50P (Harvard) | Free | ~92–155 hrs | ⬜ Not Started |
| 2 | [Classical ML](02-classical-ml/) | Regression, SVMs, Trees, Ensembles, Clustering, PCA | ISLR 2nd Ed. + Stanford edX | Free | ~145–270 hrs | ⬜ Not Started |
| 3 | [Deep Learning Foundations](03-deep-learning/) | Backprop from scratch, CNNs, RNNs, Optimization | Karpathy — Neural Networks: Zero to Hero | Free | ~110 hrs | ⬜ Not Started |
| 4 | [Modern Architectures](04-modern-architectures/) | Transformers, Attention, Self-supervised Learning | Stanford CS224n (2024) | Free | ~150 hrs | ⬜ Not Started |
| 5 | [MLOps](05-mlops/) | Deployment, Experiment Tracking, Pipelines, Monitoring | Made With ML | Free | ~120 hrs | ⬜ Not Started |
| 6 | [Specialization](06-specialization/) | Arabic NLP + Business Analytics / CRM | CS224n (NLP) + FPP (Forecasting) | Free | ~200+ hrs | ⬜ Not Started |

**Total estimated investment: ~970–1,095 hours ≈ 12–18 months at 15–20 hrs/week**

---

## 🧭 Philosophy

This roadmap is built on three principles:

1. **Math before magic** — understand *why* gradient descent converges before using Adam; derive backpropagation before importing PyTorch autograd
2. **Free first** — the internet's best ML education is free; paid resources are only cited where they genuinely fill a gap
3. **Curate, don't dump** — one primary source per stage, max two supplementary; deliberate rejection of inferior alternatives is documented

---

## 🔬 Research Methodology

Each stage was researched by:
- Cross-checking Reddit (r/MachineLearning, r/learnmachinelearning), Hacker News, and university syllabi
- Verifying currency (post-2020 preferred; pre-2016 DL materials rejected as primary)
- Assessing math depth (does it derive things, or hand-wave?)
- Confirming cost, access, prerequisites, and format

*Research conducted: July 2026*

---

## 📊 Total Cost Breakdown

| Stage | Primary Cost | Supplementary Cost |
|-------|-------------|-------------------|
| Stage 0 | Free | Free |
| Stage 1 | Free | Free |
| Stage 2 | Free (audit) | Free or ~$100–237 (Ng cert, optional) |
| Stage 3 | Free | Free |
| Stage 4 | Free | Free / ~$60 (Raschka book, optional) |
| Stage 5 | Free | Free |
| Stage 6 | Free | Free |
| **TOTAL** | **$0** | **$0–$297 optional** |

---

## 📁 Repository Structure

```
omar-badr-ml-roadmap/
├── README.md                    ← This file
├── PROGRESS.md                  ← Global progress tracker
├── 00-math-foundations/
│   ├── README.md
│   ├── sources.md
│   └── progress.md
├── 01-programming-tools/
│   ├── README.md
│   ├── sources.md
│   └── progress.md
├── 02-classical-ml/
│   ├── README.md
│   ├── sources.md
│   └── progress.md
├── 03-deep-learning/
│   ├── README.md
│   ├── sources.md
│   └── progress.md
├── 04-modern-architectures/
│   ├── README.md
│   ├── sources.md
│   └── progress.md
├── 05-mlops/
│   ├── README.md
│   ├── sources.md
│   └── progress.md
└── 06-specialization/
    ├── README.md
    ├── sources.md
    └── progress.md
```

---

*Built with deep research across YouTube channels, university OCW, MOOCs, textbooks, and community discussions. Math-first. Free-first. Omar Ahmed Badr-first.*
