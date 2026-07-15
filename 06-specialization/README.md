# Stage 6 — Specialization

## Two Tracks

This stage splits into two parallel specializations based on your existing work context:

---

## 🌍 Track 6A: Arabic NLP

**Background:** You're working with Arabic language data (CRM systems, customer text, analytics). This track builds deep Arabic NLP competency — from understanding why Arabic is uniquely challenging for NLP to fine-tuning production models.

### Why Arabic NLP is Different
Arabic presents unique challenges that no general NLP course covers:
- **Morphological richness:** One Arabic root can generate hundreds of word forms
- **Orthographic ambiguity:** Short vowels often omitted (MSA); context-dependent meaning
- **Dialect variation:** MSA (Modern Standard Arabic) vs. Egyptian, Gulf, Levantine, Maghrebi dialects
- **Right-to-left script:** Tokenization and preprocessing pipelines behave differently
- **Data scarcity:** Arabic NLP benchmarks are smaller than English; models less robust

### Learning Goals (Track 6A)
By the end of Track 6A:
- ✅ Understand Arabic-specific tokenization challenges (morphology, clitics)
- ✅ Preprocess Arabic text correctly (ArabertPreprocessor + CAMeL Tools)
- ✅ Fine-tune AraBERT/MARBERT for text classification in PyTorch
- ✅ Evaluate on ArabicNLP benchmark tasks (NER, sentiment, classification)
- ✅ Build and deploy an Arabic text classification API

### Arabic Model Hierarchy (Most → Least Important to Know)
1. `aubmindlab/bert-base-arabertv2` — Best for MSA tasks
2. `UBC-NLP/MARBERTv2` — Best for dialectal Arabic / social media
3. `CAMeL-Lab/bert-base-arabic-camelbert-mix` — Good for mixed dialect/MSA
4. `inceptionai/jais-13b` — Arabic-first LLM (2024, Inception AI)

### Arabic NLP Fine-tuning Stack (Recommended)
```
Preprocessing:   CAMeL Tools + ArabertPreprocessor
Model:           MARBERTv2 (dialectal) or AraBERTv2 (MSA)
Training:        HuggingFace Trainer API + W&B logging
Deployment:      FastAPI + Docker (learned in Stage 5)
```

### Time Estimate (Track 6A)
| Resource | Hours |
|----------|-------|
| Stanford CS224n (if not done in Stage 4) | ~80–120 hrs |
| HuggingFace LLM Course | ~40–60 hrs |
| CAMeL Tools docs + notebooks | ~15–20 hrs |
| Arabic NLP projects | ~40–80 hrs |
| **Total** | **~175–280 hrs** |

---

## 📊 Track 6B: Business Analytics / CRM

**Background:** Your existing RFM and customer segmentation work. This track deepens forecasting, survival analysis, and A/B testing skills.

### Learning Goals (Track 6B)
By the end of Track 6B:
- ✅ Build and evaluate ARIMA, ETS, and Prophet forecasting models
- ✅ Implement RFM scoring and segment customers with K-Means
- ✅ Run survival analysis (Kaplan-Meier, Cox proportional hazard) for churn
- ✅ Design and analyze A/B tests with proper statistical power
- ✅ Build customer lifetime value (LTV) models

### Time Estimate (Track 6B)
| Resource | Hours |
|----------|-------|
| Forecasting: Principles & Practice (Hyndman) | ~40–60 hrs |
| Kaggle Notebooks (RFM, segmentation, survival, A/B) | ~25–40 hrs |
| lifelines + Prophet + pingouin docs | ~10–15 hrs |
| **Total** | **~75–115 hrs** |

---

## Notes

- Both tracks can be pursued in parallel — they address different professional contexts
- Track 6A directly builds on Stage 4 (Transformers) and Stage 5 (MLOps deployment)
- Track 6B builds on Stage 2 (Classical ML) and Stage 0 (Statistics)
- **Windows note for CAMeL Tools:** Requires Rust compiler. Install via https://rustup.rs before `pip install camel-tools`
