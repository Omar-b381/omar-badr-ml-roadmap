# Stage 4 — Modern Architectures

## What This Stage Covers

The Transformer era. Everything since 2017 traces back to "Attention Is All You Need." This stage makes you fully literate in attention mechanisms, the full transformer architecture, and how BERT/GPT-style pretraining works.

| Topic | Covered By |
|-------|-----------|
| Self-attention (scaled dot-product) | Karpathy "Let's build GPT" + CS224n Lecture 8 |
| Multi-head attention | CS224n + Umar Jamil full encoder-decoder |
| Positional encoding | All primary sources |
| Transformer encoder (BERT-style) | CS224n + Harvard Annotated Transformer |
| Transformer decoder (GPT-style) | Karpathy nanoGPT + Raschka |
| Encoder-decoder (T5-style) | Umar Jamil tutorial + Harvard Annotated Transformer |
| Pretraining objectives (masked LM, CLM) | CS224n Lectures 9–10 |
| Self-supervised learning (BERT/GPT pretraining) | CS224n + Raschka Chapters 5–7 |
| Embeddings (word, positional, token) | CS224n Lectures 1–5 |
| Vision Transformers (ViT) | CS224n (connections covered) |
| Fine-tuning + instruction tuning | Raschka Chapters 6–7 + HF course |

---

## Learning Goals

By the end of Stage 4, you should be able to:

- ✅ Derive scaled dot-product attention from first principles
- ✅ Explain why masking is needed in decoder self-attention
- ✅ Implement multi-head attention in PyTorch from scratch
- ✅ Implement a GPT-style decoder-only transformer from scratch
- ✅ Implement the full encoder-decoder transformer from "Attention Is All You Need"
- ✅ Explain BERT's masked language modeling pretraining objective
- ✅ Explain GPT's causal language modeling pretraining objective
- ✅ Implement a fine-tuning loop for a classification task on a pretrained model
- ✅ Explain how positional encodings work (sinusoidal and learned)

---

## Time Estimate

| Resource | Hours |
|----------|-------|
| Stanford CS224n 2024 (primary) | ~80–100 hrs |
| Karpathy "Let's build GPT" (supplementary 1) | ~8 hrs |
| Raschka LLMs from Scratch (supplementary 2) | ~40–60 hrs |
| **Total** | **~128–168 hrs** |

> **Realistic pace:** 15 hrs/week → **~9–11 weeks**

---

## Study Order

```
Week 1:   Karpathy "Let's build GPT" video (natural continuation from Stage 3 Video 7)
Week 1–2: CS224n Lectures 1–5 (word embeddings, word2vec, GloVe)
Week 2–3: CS224n Lecture 8 — Self-Attention (⭐ most important lecture)
Week 3:   Read "Attention Is All You Need" paper alongside Lecture 8
Week 3–5: CS224n Lectures 9–10 (Transformers, pretraining — BERT/GPT)
Week 4:   Umar Jamil encoder-decoder video (fills encoder-decoder gap)
Week 4:   Harvard Annotated Transformer (paper-to-code annotation)
Week 5–8: CS224n Lectures 11–20 (NER, QA, LLMs, emergent abilities, RLHF)
Week 6–9: Raschka LLMs from Scratch (Chapters 1–7, code-along)
Week 9+:  HuggingFace NLP Course (practical bridge to production API)
```

---

## Notes

- **"Attention Is All You Need"** (2017 paper, arxiv.org/abs/1706.03762) is a mandatory 2–4 hour read. Best done alongside Karpathy's GPT video and CS224n Lecture 8.
- **Raschka's book code** (rasbt/LLMs-from-scratch on GitHub) is fully free. The book adds narrative depth but the GitHub + YouTube series (~17 hrs) delivers ~70% of the value for free.
- **HuggingFace NLP Course** is a practical bridge — it teaches the `transformers` API for using models in production. Very low math depth — but after CS224n you understand the internals, so this is purely learning the API.
- **CS224n 2024 YouTube situation:** The 2024 lectures are publicly available on YouTube (search "Stanford CS224N 2024"). Slides are linked from the course website.
