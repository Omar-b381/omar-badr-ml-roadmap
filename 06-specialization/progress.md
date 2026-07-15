# Stage 6 — Progress Tracker

---

## 🌍 Track 6A: Arabic NLP

### Foundations
- [ ] Read Stanford CS224n slides / notes on self-attention and pretraining (completed in Stage 4)
- [ ] Understand unique challenges of Arabic language NLP (morphology, orthography, dialects)
- [ ] Install Rust (`rustup`) and verify Cargo is working (required on Windows for CAMeL Tools)
- [ ] Install `camel-tools` via pip: `pip install camel-tools`
- [ ] Download CAMeL Tools datasets (run `camel_data -l` and download base packages)

### Hugging Face LLM Course (Practitioner's Path)
- [ ] Chapter 1: Transformer models overview
- [ ] Chapter 2: Using HuggingFace Transformers (pipelines, Tokenizer, Model)
- [ ] Chapter 3: Fine-tuning a pretrained model (Trainer API, compute_metrics)
- [ ] Chapter 4: Sharing models and tokenizers on Hugging Face Hub
- [ ] Chapter 5: Datasets library (load, split, filter, map)
- [ ] Chapter 6: Tokenizers library (BPE, WordPiece, training custom tokenizers)
- [ ] Chapter 7: Main NLP tasks (Token Classification, Translation, Summarization)
- [ ] Chapter 11: Prompt Engineering and LLM API basics
- [ ] Chapter 12: PEFT (Parameter-Efficient Fine-Tuning) and LoRA/QLoRA

### CAMeL Tools (Arabic Preprocessing)
- [ ] Notebook: Morphological Analysis and Generation
- [ ] Notebook: POS Tagging and Diacritization
- [ ] Notebook: Named Entity Recognition (NER)
- [ ] Notebook: Dialect Identification (MADAR corpus representation)
- [ ] Practice: Write custom preprocessing script wrapping CAMeL Tools normalizer and tokenizers

### AraBERT & MARBERT Fine-Tuning (Projects)
- [ ] Notebook: Load AraBERT (`aubmindlab/bert-base-arabertv2`) tokenizer and model
- [ ] Notebook: Fine-tune AraBERT on an Arabic Sentiment Analysis dataset (e.g., ASTD or AJGT) using HF Trainer
- [ ] Notebook: Log training metrics to Weights & Biases (W&B)
- [ ] Project: Fine-tune MARBERTv2 (`UBC-NLP/MARBERTv2`) on dialectal Arabic text classification (e.g., dialect classification or social media monitoring)
- [ ] Capstone: Build an Arabic NER model using CAMeL Tools + CAMeLBERT on a benchmark dataset (e.g., Wojood)
- [ ] MLOps Integration: Package your fine-tuned Arabic model in a FastAPI app inside a Docker container (refer to Stage 5 practices)

**Track 6A COMPLETE:** ⬜ — Date: ___

---

## 📊 Track 6B: Business Analytics & CRM

### Statistical Time-Series Forecasting (Hyndman's FPP)
- [ ] Read Chapter 1: Getting started with forecasting
- [ ] Read Chapter 2: Time series graphics
- [ ] Read Chapter 3: Time series decomposition (trend, seasonal, remainder)
- [ ] Read Chapter 7: Exponential smoothing (ETS models)
- [ ] Read Chapter 8: ARIMA models (stationarity, differencing, ACF/PACF, seasonality)
- [ ] Read Chapter 9: Dynamic regression (regression with ARIMA errors)
- [ ] Read Chapter 11: Forecasting hierarchical or grouped time series
- [ ] Practice: Implement ARIMA and ETS models using `statsmodels` in Python

### Applied CRM Analytics (Kaggle & lifelines)
- [ ] Project: RFM (Recency, Frequency, Monetary) analysis on UCI Online Retail II dataset
- [ ] Project: Apply K-Means clustering (Stage 2) on RFM scores to segment customers
- [ ] Project: Customer Churn Prediction using `lifelines`
  - [ ] Fit Kaplan-Meier survival curves for different customer cohorts
  - [ ] Fit Cox Proportional Hazards model to determine hazard ratios for covariates
- [ ] Project: A/B Testing Analysis
  - [ ] Formulate null and alternative hypotheses for a landing page experiment
  - [ ] Determine sample size and statistical power requirements using `statsmodels`
  - [ ] Perform t-tests / Mann-Whitney U tests / Chi-Squared tests to determine p-values using `pingouin` or `scipy.stats`
- [ ] Project: Time-Series Forecasting with Meta's Prophet
  - [ ] Load a retail sales dataset
  - [ ] Prepare columns as `ds` and `y`
  - [ ] Fit Prophet model, incorporate yearly/weekly/daily seasonalities and holidays
  - [ ] Plot forecasts and seasonal components
  - [ ] Perform cross-validation and hyperparameter tuning using Prophet diagnostic tools

**Track 6B COMPLETE:** ⬜ — Date: ___

---

## ✅ Stage 6 Sign-Off

### Track 6A (Arabic NLP)
- [ ] Can I explain why standard tokenizers (e.g., BERT WordPiece) fail on raw dialectal Arabic without preprocessing?
- [ ] Can I use CAMeL Tools to normalize and tag POS of a dialectal Arabic sentence?
- [ ] Can I write a custom preprocessing pipeline using `ArabertPreprocessor` and tokenizers?
- [ ] Can I fine-tune AraBERT/MARBERT on a custom dataset and evaluate classification scores?

### Track 6B (Business Analytics / CRM)
- [ ] Can I explain the decomposition of a time series into trend, seasonal, and irregular components?
- [ ] Can I interpret the coefficients/hazard ratios of a Cox Proportional Hazards model?
- [ ] Can I define RFM segments and segment customers using K-Means?
- [ ] Can I run a power analysis to calculate sample size for an A/B test?
- [ ] Can I fit, plot, and tune a Meta Prophet forecasting model?

**Stage 6 COMPLETE:** ⬜ — Date: ___
