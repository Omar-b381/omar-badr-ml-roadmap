# Stage 5 — Sources

## 🏆 Primary

### [Made With ML — by Goku Mohandas](https://madewithml.com)

- **Type:** Text-based lessons + Python notebooks + GitHub CI/CD workflows (self-paced)
- **Cost:** Free (core content). Optional paid cohorts available but not needed.
- **Math depth:** ⭐⭐☆☆☆ — Engineering focus, not theory-heavy (theory is done in Stages 0–4)
- **Why this one:** The gold standard free MLOps curriculum available. The only free resource that combines software engineering discipline (testing, linting, type hints) with ML deployment. Covers the full lifecycle end-to-end using a real NLP text classification pipeline as the running example. Topics covered: FastAPI deployment, MLflow tracking, testing (pytest), CI/CD (GitHub Actions), data versioning, model serving, Docker. The GitHub repo has ~37k stars and is actively maintained. **Crucially, the running example is an NLP classification pipeline** — directly transferable to Arabic NLP work in Stage 6.
- **Prerequisite:** Python (Stage 1), basic ML concepts (Stage 2), some familiarity with Git/CLI
- **Est. time:** 60–100 hours
- **GitHub:** https://github.com/GokuMohandas/Made-With-ML (~37k stars)
- **Sections:**
  1. Workspaces (git, virtual environments, code structure)
  2. Data Engineering
  3. Modeling (scikit-learn + PyTorch)
  4. Training (MLflow experiment tracking)
  5. Evaluation & Testing (pytest, behavioral testing)
  6. Serving (FastAPI, model packaging)
  7. CI/CD (GitHub Actions, automated workflows)
  8. Data & Model Monitoring

---

## 📌 Supplementary 1

### [MLOps Zoomcamp — DataTalks.Club](https://github.com/DataTalksClub/mlops-zoomcamp)

- **Type:** Video lectures (YouTube) + notebooks + homework assignments (self-paced)
- **Cost:** Free (100% — all materials on GitHub + YouTube)
- **Math depth:** ⭐☆☆☆☆ — Very tool-focused
- **Why this one:** Not on the original candidate list, but discovered during research as the best supplementary for Stage 5. Its curriculum is a point-for-point match with the Stage 5 topic list: Module 2 = MLflow, Module 3 = Prefect orchestration, Module 4 = FastAPI + Docker deployment, Module 5 = Evidently AI monitoring, Module 6 = CI/CD + GitHub Actions + Terraform. Actively maintained cohort-based course with self-paced access. Hands-on project-based (NYC taxi dataset).
- **Prerequisite:** Python, Docker basics, some ML experience (Stage 2+)
- **Est. time:** ~50–90 hours (9 weeks × 5–10 hrs/week)
- **Modules (exact match to Stage 5 topics):**
  - Module 1: Introduction to MLOps
  - Module 2: MLflow (experiment tracking)
  - Module 3: Prefect (workflow orchestration)
  - Module 4: FastAPI + Docker (deployment)
  - Module 5: Evidently AI + Prometheus + Grafana (monitoring)
  - Module 6: GitHub Actions + Terraform (CI/CD)

---

## 📌 Supplementary 2

### [Weights & Biases AI Academy](https://wandb.ai/fully-connected)

- **Type:** Short modular video courses (~2 hrs each) + code-along notebooks
- **Cost:** Free
- **Math depth:** ⭐☆☆☆☆ — Tool-focused (W&B ecosystem)
- **Why this one:** W&B is the experiment tracker of choice in NLP and ML research communities (most Arabic NLP papers log experiments on W&B, not MLflow). Learning it in Stage 5 directly benefits Stage 6A Arabic NLP fine-tuning work. Frequently updated with new courses on LLMOps, RAG, and agents (2024/2025 additions). W&B's Weave platform for LLM monitoring is also worth exploring for Stage 6.
- **Prerequisite:** Some ML experience; Python
- **Est. time:** 10–15 hrs (selected courses)
- **Courses to prioritize:**
  - Experiment tracking with W&B
  - LLM Evaluation with W&B
  - Model monitoring basics

---

## References (Keep Bookmarked)

### [MLflow Documentation](https://mlflow.org/docs/latest/)
- **Cost:** Free
- **When to use:** Reference alongside Made With ML's training section and MLOps Zoomcamp Module 2. MLflow 2.x series actively maintained. Key features: autologging, Model Registry, LLM tracing support.

### [Evidently AI Documentation](https://docs.evidentlyai.com)
- **Cost:** Free
- **When to use:** Reference alongside MLOps Zoomcamp Module 5. Quick demo: `evidently ui --demo-projects all`. Integrates with Made With ML's monitoring section.

---

## Background Reading (Optional — if accessible)

### [Designing Machine Learning Systems — Chip Huyen (O'Reilly, 2022)](https://huyenchip.com/books)
- **Cost:** ~$50–60 (O'Reilly). Not free — check library or O'Reilly subscription.
- **Math depth:** ⭐☆☆☆☆ — Systems design focus
- **Why worth reading (if accessible):** "Must-read" status among ML practitioners; holistic systems thinking; bridges research↔production gap; timeless principles for data engineering, feature stores, model monitoring, and business alignment.
- **Limitation:** Pre-LLM era (2022); not a coding guide; doesn't cover Prefect/MLflow specifically.
- **Companion:** Chip Huyen's follow-up *"AI Engineering"* (2024) covers the LLM-era equivalent (RAG, LLMOps, evaluation-driven development).

---

## ❌ Rejected Candidates

| Resource | Reason Rejected |
|----------|----------------|
| **Full Stack Deep Learning (FSDL)** | Core MLOps course is archived (2022 vintage, tooling outdated). The LLM Bootcamp (2023) covers LLMOps but doesn't address the Stage 5 tool list comprehensively. MLOps Zoomcamp is strictly superior for Stage 5 purposes. |
| **DataCamp MLOps Track** | Paid (~$14–25/month); sandboxed browser environment doesn't transfer to real-world experience. Practitioners consistently rate it insufficient for job-readiness alone. Given the quality of free alternatives (Made With ML + MLOps Zoomcamp), the ROI is poor. |
