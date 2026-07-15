# Stage 5 — MLOps / Applied Production Skills

## What This Stage Covers

Models that live only in Jupyter notebooks don't create value. This stage bridges research and production: packaging, deploying, tracking, monitoring, and automating ML systems.

| Topic | Tools Covered |
|-------|-------------|
| Experiment tracking | MLflow, Weights & Biases |
| Model deployment | FastAPI, Docker, REST APIs |
| Data pipelines | Prefect (orchestration), DVC (data versioning) |
| Model monitoring | Evidently AI, Prometheus, Grafana |
| CI/CD for ML | GitHub Actions, automated testing |
| Code quality | pytest, linting, type hints in ML projects |
| Feature stores | Feast (concepts) |
| Containerization | Docker, Docker Compose |

---

## Learning Goals

By the end of Stage 5, you should be able to:

- ✅ Build an end-to-end ML pipeline (data ingestion → training → evaluation → serving)
- ✅ Track experiments (parameters, metrics, artifacts) with MLflow
- ✅ Wrap a model in a FastAPI REST endpoint
- ✅ Containerize an ML application with Docker
- ✅ Build an automated CI/CD pipeline for model retraining with GitHub Actions
- ✅ Set up model monitoring for data drift using Evidently AI
- ✅ Orchestrate a data pipeline with Prefect
- ✅ Write unit tests for ML components with pytest

---

## Time Estimate

| Resource | Hours |
|----------|-------|
| Made With ML (primary) | ~60–100 hrs |
| MLOps Zoomcamp (supplementary 1) | ~50–90 hrs |
| W&B AI Academy (supplementary 2) | ~10–15 hrs |
| **Total** | **~120–205 hrs** |

> **Realistic pace:** 15 hrs/week → **~2–3 months**

---

## Study Order

```
Weeks 1–6:   Made With ML (PRIMARY) — build end-to-end NLP pipeline
Parallel:    MLOps Zoomcamp (SUPP 1) — hands-on tool practice alongside
Weeks 5–7:   W&B AI Academy courses (SUPP 2) — when working on experiment tracking
Reference:   MLflow docs (https://mlflow.org/docs/latest/) — alongside relevant sections
Reference:   Evidently AI docs (https://docs.evidentlyai.com) — Module 5 of Zoomcamp
```

---

## Notes

- **Made With ML's running example is an NLP classification pipeline** — the exact same architecture you'll use for Arabic NLP fine-tuning in Stage 6. Intentional alignment.
- **W&B is the experiment tracker of choice in NLP research** — most Arabic NLP papers report experiments tracked on W&B. Learning it in Stage 5 pays dividends in Stage 6A.
- **FSDL (Full Stack Deep Learning) is NOT recommended** — its core MLOps course is effectively archived (last updated 2022); the "LLM Bootcamp" (2023) remains useful but doesn't cover Stage 5's tool list comprehensively. MLOps Zoomcamp is strictly superior for this stage.
- **DataCamp MLOps track is NOT recommended** — paid subscription for sandboxed exercises that don't transfer to real-world environments. The free alternatives are better.
- **Chip Huyen's "Designing Machine Learning Systems"** (O'Reilly, 2022): Worth reading if accessible (library, O'Reilly subscription, or used copy). Not essential — the free resources cover tooling far better. Good for systems-thinking perspective.
