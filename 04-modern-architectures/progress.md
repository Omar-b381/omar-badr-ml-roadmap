# Stage 4 — Progress Tracker

---

## Karpathy "Let's build GPT" (SUPPLEMENTARY 1 — but do it FIRST as Stage 3→4 bridge)

- [ ] Watch full video (~2 hrs): https://www.youtube.com/watch?v=kCc8FmEb1nY
- [ ] Implement self-attention from scratch (scaled dot-product)
- [ ] Implement multi-head attention
- [ ] Add positional encoding
- [ ] Implement the decoder block (LayerNorm, FFN, residual)
- [ ] Assemble full GPT model
- [ ] Train on Tiny Shakespeare (~1MB) on local machine or Colab
- [ ] Read "Attention Is All You Need" paper sections 3.1–3.4 alongside this

**Karpathy GPT COMPLETE:** ⬜ — Date: ___

---

## Stanford CS224n 2024 (PRIMARY)

### Lectures 1–5: Word Embeddings
- [ ] Lecture 1: Intro to NLP + word meaning
- [ ] Lecture 2: Word vectors (word2vec) — derivation of skip-gram objective
- [ ] Lecture 3: Word window classification, neural networks
- [ ] Lecture 4: Backprop in NLP
- [ ] Lecture 5: Linguistics, syntactic structure, dependency parsing
- [ ] Finish reading "Attention Is All You Need" paper completely

### Lectures 6–8: Transformers (Core)
- [ ] Lecture 6: Language models and recurrent networks
- [ ] Lecture 7: Seq2Seq, machine translation
- [ ] Lecture 8: Self-Attention and Transformers ⭐ (Most important lecture — watch twice)
  - [ ] Understand scaled dot-product attention derivation
  - [ ] Understand why masking is needed in decoder
  - [ ] Understand multi-head attention intuition
  - [ ] Read slides Section 3 of "Attention Is All You Need" alongside

### Lectures 9–10: Pretraining + BERT/GPT
- [ ] Lecture 9: Pretraining (self-supervised objectives)
  - [ ] Understand masked language modeling (BERT)
  - [ ] Understand causal language modeling (GPT)
  - [ ] Understand next sentence prediction (BERT)
- [ ] Lecture 10: Transformers in context (scale, emergent abilities)
- [ ] Umar Jamil encoder-decoder video (watch alongside Lecture 9 for encoder-decoder gap)
- [ ] Harvard Annotated Transformer walkthrough (alongside Lectures 9–10)

### Lectures 11–15: NLP Applications
- [ ] Lecture 11: Question answering
- [ ] Lecture 12: Natural language generation
- [ ] Lecture 13: Coreference resolution
- [ ] Lecture 14: Analysis and interpretability
- [ ] Lecture 15: Model efficiency + ethics

### Lectures 16–20: Advanced Topics
- [ ] Lecture 16: Code generation + instruction following
- [ ] Lecture 17: Large language models in practice
- [ ] Lecture 18: RLHF and alignment
- [ ] Lecture 19: Multimodal models (ViT connections)
- [ ] Lecture 20: Future of NLP

**CS224n 2024 COMPLETE:** ⬜ — Date: ___

---

## Raschka — LLMs from Scratch (SUPPLEMENTARY 2)

### Part 1: Building GPT-2 from Scratch
- [ ] Ch. 1–2: Tokenization — BPE implementation, data loading
- [ ] Ch. 3: Coding attention mechanisms (chapter by chapter)
  - [ ] Simplified self-attention
  - [ ] Self-attention with trainable weights
  - [ ] Multi-head attention class
- [ ] Ch. 4: Full GPT-2 architecture assembly
  - [ ] Layer normalization
  - [ ] GELU activation function
  - [ ] Feed-forward module
  - [ ] Shortcut connections
  - [ ] Transformer block
  - [ ] Full GPT model class

### Part 2: Pretraining and Fine-tuning
- [ ] Ch. 5: Pretraining on unlabeled data
  - [ ] Text generation with greedy decoding + sampling
  - [ ] Training loop with gradient clipping
  - [ ] Loading pretrained GPT-2 weights from OpenAI
- [ ] Ch. 6: Fine-tuning for classification
  - [ ] Adding classification head
  - [ ] Training on spam dataset
- [ ] Ch. 7: Instruction fine-tuning
  - [ ] Alpaca-style dataset format
  - [ ] RLHF-adjacent reward modeling intuition

**Raschka LLMs from Scratch COMPLETE:** ⬜ — Date: ___

---

## Supplementary References

### "Attention Is All You Need" Paper
- [ ] Section 3.1: Encoder-Decoder architecture overview
- [ ] Section 3.2: Attention — scaled dot-product, multi-head
- [ ] Section 3.3: Position-wise feed-forward networks
- [ ] Section 3.4: Embeddings and positional encoding
- [ ] Section 3.5: Why attention? (complexity table)
- [ ] Read entire paper at least once carefully

### Harvard Annotated Transformer
- [ ] Work through full notebook: https://nlp.seas.harvard.edu/annotated-transformer/
- [ ] Understand encoder: embedding → positional encoding → multi-head self-attention → FFN
- [ ] Understand decoder: masked self-attention → cross-attention → FFN
- [ ] Understand the label smoothing and learning rate warmup schedule

### Umar Jamil — Transformer from scratch
- [ ] Watch full video: https://www.youtube.com/watch?v=ISNdQcPhsts
- [ ] Code along with full encoder-decoder implementation
- [ ] Understand masking for encoder (padding mask) vs decoder (causal + padding mask)

### HuggingFace LLM Course (use after theory is solid)
- [ ] Chapter 1: Transformer models overview
- [ ] Chapter 2: Using HuggingFace Transformers
- [ ] Chapter 3: Fine-tuning a pretrained model (Trainer API)
- [ ] Chapter 4: Sharing models on Hub
- [ ] Chapter 5: HuggingFace Datasets library

---

## ✅ Stage 4 Sign-Off

- [ ] Can I derive scaled dot-product attention from first principles?
- [ ] Can I implement multi-head attention in PyTorch from scratch?
- [ ] Can I implement a full GPT-style decoder-only transformer?
- [ ] Can I explain the difference between BERT (masked LM) and GPT (causal LM) pretraining?
- [ ] Can I fine-tune a pretrained BERT model for classification using the HF Trainer API?
- [ ] Can I explain why sinusoidal positional encodings work?
- [ ] Can I implement BPE tokenization conceptually (not necessarily from scratch)?

**Stage 4 COMPLETE → Ready for Stage 5:** ⬜ — Date: ___
