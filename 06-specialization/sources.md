# Stage 6 — Sources

---

# 🌍 Track 6A: Arabic NLP

## 🏆 Primary (Track 6A)

### [Stanford CS224n — NLP with Deep Learning (2024)](https://web.stanford.edu/class/cs224n/)

- **Type:** Video lectures (~20 × 80 min) + slides + assignments
- **Cost:** Free (YouTube + course website)
- **Math depth:** ⭐⭐⭐⭐⭐ — Full mathematical treatment of transformers, pretraining, NER, fine-tuning, RLHF
- **Why this one:** The theoretical backbone needed to properly understand, fine-tune, and troubleshoot Arabic BERT variants. Without this foundation, Arabic NLP fine-tuning becomes cargo-culting. The 2024 YouTube playlist covers modern LLM fine-tuning topics directly relevant to Stage 6A work. Without CS224n, you won't understand *why* AraBERT needs the ArabertPreprocessor, or *why* MARBERTv2 generalizes better to dialectal Arabic. **Note:** If covered in Stage 4, this is already complete — Stage 6A primarily uses HF Course + CAMeL Tools.
- **Prerequisite:** Stage 3 (deep learning) + Stage 4 (transformers)
- **Est. time:** ~80–120 hrs (or skip if completed in Stage 4)

---

## 📌 Supplementary 1 (Track 6A)

### [Hugging Face LLM Course](https://huggingface.co/learn)

- **Type:** Interactive web lessons + Colab notebooks (self-paced)
- **Cost:** Free (rebranded "LLM Course" in 2025 with new fine-tuning and evaluation chapters)
- **Math depth:** ⭐⭐☆☆☆ — API-focused; teaches the exact API used to fine-tune Arabic models
- **Why this one:** The essential practitioner's toolkit. CS224n gives you the "why"; HF course gives you the "how" with the exact libraries you'll use. AraBERT, MARBERT, CAMeLBERT are all on the HF Hub and use identical `transformers` API patterns. Arabic preprocessing via `ArabertPreprocessor` slots into HF pipelines. Actively updated — includes DeepSeek R1, LoRA/PEFT fine-tuning techniques, evaluation-driven development.
- **Arabic-specific value:** The skills are directly transferable — Arabic models on HF Hub use the same fine-tuning code as English models, with the addition of Arabic preprocessing.
- **Prerequisite:** PyTorch basics, Stage 3 complete
- **Est. time:** ~40–60 hrs
- **Key chapters:**
  - Chapters 1–4: Transformers API, tokenization (including Arabic subword tokenization), fine-tuning
  - Chapter 5: Datasets library (for Arabic NLP datasets)
  - Chapters 6–9: Advanced fine-tuning (PEFT, LoRA), evaluation, deployment

---

## 📌 Supplementary 2 (Track 6A)

### [CAMeL Tools — Documentation + Notebooks](https://github.com/CAMeL-Lab/camel_tools)

- **Type:** Python library + docs + Colab notebooks + YouTube "Arabic NLP Series"
- **Cost:** Free
- **Math depth:** ⭐☆☆☆☆ — Tool-focused; the underlying morphological analysis is linguistic, not mathematical
- **Why this one:** The ONLY comprehensive Arabic-specific NLP library with active maintenance from an academic lab (NYU Abu Dhabi). Handles MSA, dialectal, and Classical Arabic variants. CAMeLBERT models are SOTA on several Arabic NLP benchmarks. Addresses the unique challenges of Arabic (morphological richness, orthographic ambiguity, dialect variation) that no general NLP course covers. Non-negotiable for serious Arabic NLP work — no other resource addresses Arabic-specific preprocessing.
- **Prerequisite:** Python, HF Transformers basics
- **Est. time:** ~15–20 hrs
- **Docs:** https://camel-tools.readthedocs.io
- **GitHub:** https://github.com/CAMeL-Lab/camel_tools
- **⚠️ Windows note:** Requires Rust compiler. Install via https://rustup.rs BEFORE running `pip install camel-tools`
- **YouTube:** Search "CAMeL Lab Arabic NLP Series" (episodes 9, 16, 17)

---

## Arabic NLP References

### [AraBERT — GitHub + HuggingFace](https://github.com/aub-mind/arabert)
- **Cost:** Free
- **HF Hub:** https://huggingface.co/aubmindlab
- **Key models:**
  - `aubmindlab/bert-base-arabertv2` (MSA, most widely used)
  - `aubmindlab/bert-large-arabertv2` (larger MSA model)
  - `UBC-NLP/MARBERTv2` (dialectal Arabic — best for social media)
  - `CAMeL-Lab/bert-base-arabic-camelbert-mix` (mixed dialect/MSA)
- **Key notebook:** `AraBERT_Text_Classification_with_HF_Trainer_Pytorch_GPU.ipynb` in the GitHub repo
- **Usage:** Start all Arabic NLP projects with `ArabertPreprocessor` before tokenizing

### [ACL Anthology — ArabicNLP Conference](https://aclanthology.org)
- **Cost:** Free
- **How to find:** Search "ArabicNLP 2024" or "WANLP" for recent Arabic NLP papers
- **Key shared tasks (2024):** WojoodNER 2024 (Arabic NER), AFTD (text classification)
- **Use:** Browse papers from ArabicNLP 2023–2025 for SOTA methods and benchmarks

### [JAIS — Arabic-First LLM (Inception AI, 2024)](https://huggingface.co/inceptionai)
- **Models:** `inceptionai/jais-13b`, `inceptionai/jais-30b-chat`
- **Use:** When you want to go beyond fine-tuning encoder models and work with generative Arabic LLMs

---

# 📊 Track 6B: Business Analytics / CRM

## 🏆 Primary (Track 6B)

### [Forecasting: Principles and Practice — Hyndman & Athanasopoulos (Python Edition)](https://otexts.com/fpppy)

- **Type:** Free online textbook with integrated Python code
- **Cost:** Free
- **Math depth:** ⭐⭐⭐☆☆ — Statistical methods explained with underlying math; ETS models derived, ARIMA shown with full ARMA notation; enough rigor to understand Prophet's decomposition
- **Why this one:** The definitive open-access forecasting textbook. Unmatched depth-to-accessibility ratio. Free, authoritative, Python-usable. Essential for understanding WHY forecasting methods work (not just calling `prophet.fit()`). Covers ETS/ARIMA fundamentals that explain Prophet's decomposition model. Regularly cited in industry forecasting. The Python edition (2024) directly replaces the R-centric 3rd edition for Python practitioners.
- **Prerequisite:** Basic statistics (Stage 0), Python/Pandas (Stage 1)
- **Est. time:** ~40–60 hrs
- **Chapter guide:**
  - Ch. 1–3: Time series basics, graphics, decomposition
  - Ch. 7: Exponential smoothing (ETS models)
  - Ch. 8: ARIMA
  - Ch. 9: Regression with time series errors
  - Ch. 11: Forecasting hierarchical series

---

## 📌 Supplementary 1 (Track 6B)

### [Kaggle Notebooks — RFM, Segmentation, Survival Analysis, A/B Testing](https://www.kaggle.com)

- **Type:** Community Jupyter notebooks (runnable in Kaggle cloud)
- **Cost:** Free
- **Math depth:** ⭐⭐☆☆☆ — Applied focus; code-first
- **Why this one:** The fastest way to build practical CRM/business analytics skills. Hyndman for theory; Kaggle notebooks for hands-on implementation across all specific topics. Real-world datasets readily available.
- **Prerequisite:** Python, Pandas, Stage 2 classical ML (K-Means, clustering)
- **Est. time:** ~25–40 hrs (curated notebooks)
- **Key searches:**
  - `"Customer Segmentation RFM UCI"` — RFM scoring + K-Means on UCI Online Retail II dataset
  - `"Survival Analysis Telco Churn lifelines"` — Kaplan-Meier, Cox PH for churn
  - `"A/B Testing Python scipy"` — t-tests, Mann-Whitney, chi-square for A/B
  - `"Customer Lifetime Value LTV"` — LTV modeling approaches

---

## 📌 Supplementary 2 (Track 6B)

### [lifelines docs](https://lifelines.readthedocs.io) + [Prophet docs](https://facebook.github.io/prophet/) + [pingouin docs](https://pingouin-stats.org)

- **Type:** Official library documentation + Python examples
- **Cost:** Free
- **Math depth:** ⭐☆☆☆☆ — API usage; FPP gives the conceptual depth
- **Why this combination:** After learning survival analysis theory from lifelines docs and forecasting theory from Hyndman, these docs take only 1–2 days each to master the API. Prophet's sklearn-like API (`fit`/`predict`) handles business time-series with missing data and outliers automatically. Pingouin provides a clean API for statistical testing (t-tests, ANOVA, correlation) with automatic effect size reporting.
- **Est. time:** ~10–15 hrs across all three

---

## ❌ Rejected Candidates (Track 6B)

| Resource | Reason Rejected |
|----------|----------------|
| **Kaggle alone (primary)** | Kaggle notebooks are applied-first with no underlying statistical derivation. Need Hyndman for the "why" behind ETS and ARIMA |
| **Prophet alone (primary)** | Prophet is a tool; Hyndman explains the additive decomposition model Prophet is built on |
| **DataCamp Data Science track** | Paid; narrower coverage than the free stack |
