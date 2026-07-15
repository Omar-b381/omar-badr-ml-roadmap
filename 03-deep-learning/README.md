# Stage 3 — Deep Learning Foundations

## What This Stage Covers

This is where you *build* the engine. No importing `torch.autograd` until you've written it yourself. Every concept in this stage is derived in code — backpropagation as a manual computational graph walk, BatchNorm internals, and the full PyTorch-from-scratch journey.

| Topic | How It's Taught |
|-------|----------------|
| Backpropagation | Built from scratch: derivative of each node in a computational graph (Karpathy `micrograd`) |
| Multi-layer Perceptrons | Built incrementally: neuron → layer → MLP → training loop |
| Activations & Gradients | Dead neurons, vanishing/exploding gradients, activation function comparison |
| Batch Normalization | Derived and implemented from scratch; internal mechanics explained |
| CNNs | Andrew Ng Course 4 (architecture) + CS231n notes (backprop through conv layers) |
| RNNs / LSTMs | Andrew Ng Course 5 + CS231n Assignment 2 (implement vanilla RNN + LSTM in NumPy) |
| Optimization | Adam, SGD variants, momentum, learning rate decay — Ng Course 2 |
| Regularization | Dropout, L2 weight decay, early stopping |

---

## Learning Goals

By the end of Stage 3, you should be able to:

- ✅ Build a scalar-valued autograd engine in pure Python (like `micrograd`)
- ✅ Manually compute the gradient of a simple 2-layer network by hand
- ✅ Implement a full MLP training loop in PyTorch from scratch
- ✅ Explain how BatchNorm works internally (forward pass, backward pass)
- ✅ Implement a vanilla RNN and LSTM in NumPy from scratch
- ✅ Explain why Adam typically outperforms vanilla SGD
- ✅ Implement dropout and explain what it's doing to the computation graph
- ✅ Build and train a simple CNN for image classification

---

## Time Estimate

| Resource | Hours |
|----------|-------|
| Karpathy Zero to Hero (primary) | ~50 hrs (incl. coding) |
| Andrew Ng DLS Courses 2 + 4 (supplementary 1) | ~30 hrs |
| CS231n Notes + Assignment 2 (supplementary 2) | ~30 hrs |
| **Total** | **~110 hrs** |

> **Realistic pace:** 15 hrs/week → **~7 weeks**

---

## Study Order

```
Week 1:    MIT 6.S191 (optional — 15 hrs) — orientation sweep, big picture overview
Week 1–2:  Karpathy Video 1 (micrograd + backprop) — THE most important lesson
Week 2–4:  Karpathy Videos 2–4 (MLP, activations, BatchNorm)
Week 4–5:  Karpathy Videos 5–6 (WaveNet, makemore)
Week 5:    Karpathy Video 7 (Let's build GPT — bridge to Stage 4)
Week 4–6:  Andrew Ng DLS Course 2 (Adam, SGD, dropout, BatchNorm — structured)
Week 5–7:  Andrew Ng DLS Course 4 (CNNs — the Karpathy gap fill)
Week 6–7:  CS231n Notes (backpropagation computational graphs)
Week 7:    CS231n Assignment 2 (vanilla RNN + LSTM in NumPy)
```

---

## Notes

- **Karpathy's series intentionally omits standalone CNNs.** This is acknowledged by Karpathy himself. Use Ng Course 4 and CS231n notes to fill this gap.
- **CS231n video situation:** Recent lecture videos (2022–2024) are restricted to enrolled Stanford students. Only 2017 lectures are on YouTube. However, the **notes and slides are fully public** — the 2024 Spring slides are available on the course website. The notes are the higher-value component anyway.
- **fast.ai Part 2** is an optional enrichment for seeing how expert practitioners write DL code from scratch (including BatchNorm and backprop in `miniai`). Not required.
- **Goodfellow et al. "Deep Learning" book** (deeplearningbook.org) — use Chapters 6–8 as a mathematical reference for regularization and optimization theory when Ng feels too shallow.
