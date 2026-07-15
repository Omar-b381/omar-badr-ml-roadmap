# Stage 4 — Sources

## 🏆 Primary

### [Stanford CS224n — NLP with Deep Learning (2024)](https://web.stanford.edu/class/cs224n/)

- **Type:** Video lectures (~20 × 80 min) + slides + assignments (self-study)
- **Cost:** Free (lectures on YouTube; slides/assignments on course website). Professional XCS224N version: ~$1,500+
- **Math depth:** ⭐⭐⭐⭐⭐ — Stanford PhD-level course; full mathematical treatment of attention, transformer training, pretraining objectives, RLHF, emergent capabilities; proofs and rigorous notation throughout
- **Why this one:** The only resource in the candidate list that covers the complete Stage 4 syllabus — self-attention, multi-head attention, transformer architecture, positional encoding, self-supervised learning (BERT/GPT pretraining), embeddings, AND vision transformer connections — at a mathematically rigorous level, with current (2024) content. The slides alone are worth the effort: Lecture 8 (self-attention) and the BERT/GPT pretraining lectures are some of the best-written lecture slides in the field. **Updated annually** — the 2024 edition explicitly covers modern LLMs, emergent capabilities, RLHF, and code generation. The 80–100 hour commitment pays off in deep, durable understanding. **Crucially, this is all free** — the XCS224N professional version is over $1,500, but the YouTube lectures + slides are identical.
- **Prerequisite:** Strong ML fundamentals (Stage 0 math + Stage 2 classical ML + Stage 3 backprop); Python/PyTorch
- **Est. time:** ~80–100 hrs (20 lectures + assignments)
- **2024 YouTube:** Search "Stanford CS224N 2024 YouTube"
- **Course website:** https://web.stanford.edu/class/cs224n/

---

## 📌 Supplementary 1

### [Andrej Karpathy — "Let's build GPT from scratch"](https://www.youtube.com/watch?v=kCc8FmEb1nY)

- **Type:** Single YouTube video (1 hr 56 min) + companion nanoGPT codebase
- **Cost:** Free
- **Math depth:** ⭐⭐⭐⭐☆ — Derives self-attention from scratch with full dimensional analysis; derives positional encoding; explains why scaled dot-product attention works intuitively and mathematically
- **Why this one:** ~2 hours of video that gives bottom-up intuition for exactly how self-attention and the GPT architecture work in code. CS224n teaches the theory rigorously; Karpathy makes you actually *feel* it by building it character-by-character. Must be watched alongside CS224n's transformer lectures — they are perfect complements. Also serves as a natural bridge from Stage 3 (the Zero to Hero series). Called "the best single DL video on YouTube" repeatedly in the ML community — HackerNews front-page upon release.
- **Prerequisite:** Stage 3 Karpathy Zero to Hero complete (or this is Video 7 of the same series)
- **Est. time:** ~2 hrs video; ~6–10 hrs coding along
- **nanoGPT:** https://github.com/karpathy/nanoGPT

---

## 📌 Supplementary 2

### [Sebastian Raschka — "Build a Large Language Model (From Scratch)"](https://github.com/rasbt/LLMs-from-scratch)

- **Type:** Book (~$60 Manning) + free GitHub code + free YouTube series (~17 hrs, 48 episodes)
- **Cost:** GitHub code + YouTube series = **Free**. Book: ~$59.99 (Manning)
- **Math depth:** ⭐⭐⭐⭐☆ — More rigorous than Karpathy in coverage of BPE tokenization, pretraining objectives, and fine-tuning; includes instruction-following and RLHF-adjacent content
- **Why this one:** For learners who want to go beyond the GPT video and understand the full LLM lifecycle (pretraining → fine-tuning → instruction tuning), Raschka's 2024 resource is the most current and comprehensive available. Fills every gap left by Karpathy's video: BPE tokenization, pretraining objectives, fine-tuning loops, and loading real GPT-2 weights. The models can be run locally (no cloud GPU required). Most thorough current (2024) book-length resource for the full LLM pipeline.
- **Prerequisite:** Stage 3 complete; PyTorch basics
- **Est. time:** ~40–60 hrs (code-along with GitHub + YouTube)
- **GitHub:** https://github.com/rasbt/LLMs-from-scratch
- **Chapter breakdown:**
  - Ch. 1–2: Tokenization (BPE), data loading
  - Ch. 3–4: Attention mechanisms, GPT-2 architecture
  - Ch. 5: Pretraining from scratch
  - Ch. 6: Fine-tuning for classification
  - Ch. 7: Instruction fine-tuning (Alpaca-style)

---

## Mandatory Reference (Read Alongside Primary)

### ["Attention Is All You Need" — Vaswani et al. (2017)](https://arxiv.org/abs/1706.03762)

- **Type:** 15-page academic paper
- **Cost:** Free
- **Math depth:** ⭐⭐⭐⭐⭐ — THE source; defines scaled dot-product attention, multi-head attention, and positional encoding with full mathematical notation
- **Est. time:** 2–4 hrs to read carefully; 10–20 hrs to fully annotate
- **When to read:** Alongside CS224n Lecture 8 and Karpathy's GPT video

---

## Additional Supplements

### [Harvard — The Annotated Transformer (2022 rewrite)](https://nlp.seas.harvard.edu/annotated-transformer/)
- **Cost:** Free
- **Math depth:** ⭐⭐⭐⭐☆ — Annotates every equation in the paper with corresponding working PyTorch code
- **Why useful:** Best for rigorous paper-to-code translation of the encoder-decoder architecture. The 2022 rewrite is fully PyTorch-compatible and runs on Colab.
- **Est. time:** 6–10 hrs

### [Umar Jamil — Coding a Transformer from scratch on PyTorch](https://www.youtube.com/watch?v=ISNdQcPhsts)
- **Cost:** Free | GitHub: https://github.com/hkproj/pytorch-transformer
- **Math depth:** ⭐⭐⭐⭐☆ — Full encoder-decoder transformer from "Attention Is All You Need" paper
- **Why useful:** Implements the FULL original transformer (encoder+decoder) — the complement to Karpathy's decoder-only GPT. 700,000+ views; among the most cited transformer implementation tutorials.
- **Est. time:** ~6–8 hrs (video + coding)

### [HuggingFace NLP / LLM Course](https://huggingface.co/learn)
- **Cost:** Free
- **Math depth:** ⭐⭐☆☆☆ — API-focused; almost no math
- **When to use:** AFTER Stage 4 theory is solid, as a practical bridge to using transformers in production (Trainer API, tokenization, Hub, fine-tuning). Rebranded as "LLM Course" in 2025 with chapters on DeepSeek R1, fine-tuning techniques.
- **Est. time:** ~30–40 hrs

---

## ❌ Rejected Candidates

| Resource | Reason Rejected |
|----------|----------------|
| **Karpathy "Let's build GPT" as primary** | Excellent but covers only decoder-only GPT style; doesn't cover encoder-only (BERT), encoder-decoder (T5), vision transformers, or pretraining in depth. Too narrow for full Stage 4 scope. Kept as Supplementary 1. |
| **HuggingFace NLP Course as primary** | Math depth is essentially zero — it's a library tutorial, not a conceptual course. Won't teach how attention works, only how to use it. Kept as practical supplement after theory is solid. |
| **Raschka book as primary** | Focuses on GPT-style only (no BERT encoder-only, no ViT); despite being the most current (2024), CS224n's breadth and rigor make it a better primary. Kept as Supplementary 2. |
