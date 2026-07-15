# Stage 3 — Sources

## 🏆 Primary

### [Andrej Karpathy — Neural Networks: Zero to Hero](https://youtube.com/playlist?list=PLAqhIrjkxbuWI23v9cThsA9GvCAUhRvKZ)

- **Type:** 7 YouTube lectures + Jupyter notebooks (code-along)
- **Cost:** Free
- **Math depth:** ⭐⭐⭐⭐☆ — Derives backpropagation manually by computing gradients of every node in a computational graph ("becoming a backprop ninja"). Covers activations, BatchNorm internals, and chain rule deeply in code. Math is code-first — not abstract proofs but genuine mathematical derivation in Python.
- **Why this one:** No other resource builds backpropagation intuition from first principles the way Karpathy does — deriving every gradient manually, automating it step-by-step, and building up to modern architectures. The progression from micrograd → makemore → GPT is a continuous, unbroken chain of understanding. The "Becoming a Backprop Ninja" video alone covers more ground than most full courses. Karpathy's credibility (ex-OpenAI/Tesla AI director) is elite. GitHub repo has tens of thousands of stars and is actively referenced across academia and industry.
- **Prerequisite:** High-school calculus (derivatives), Python basics (Stage 1), some ML intuition (Stage 2)
- **Est. time:** ~19 hrs video; ~40–60 hrs with coding exercises
- **GitHub:** https://github.com/karpathy/nn-zero-to-hero
- **Lecture breakdown:**
  - Video 1: Backprop from scratch → builds `micrograd` (a tiny autograd engine in pure Python)
  - Videos 2–4: MLP, activations & gradients, BatchNorm from scratch
  - Videos 5–6: WaveNet-style architectures (makemore series)
  - Video 7: Builds GPT from scratch (bridges into Stage 4)

---

## 📌 Supplementary 1

### [Andrew Ng — Deep Learning Specialization, Courses 2 & 4 (Coursera)](https://www.coursera.org/specializations/deep-learning)

- **Type:** Video lectures + graded NumPy/TensorFlow assignments
- **Cost:** ~$49–79/month (audit free; certificate behind paywall). **Use Courses 2 and 4 only.**
- **Math depth:** ⭐⭐⭐☆☆ — Intuition-first; derives gradient descent update rules and shows optimization landscape; NumPy assignments compensate for lack of proofs
- **Why this one:** Karpathy doesn't have dedicated CNNs or RNN/LSTM lectures. Ng's Course 2 covers Adam, SGD variants, momentum, learning rate decay, dropout, and BatchNorm with structured assignments. Course 4 covers CNNs (ResNets, YOLO) — the gap Karpathy intentionally leaves. Millions of completions; industry-respected. **Skip Course 3 entirely** (project management content, minimal learning value). Course 5 (Sequence Models) is worth skimming for RNNs/LSTMs before going to Stage 4.
- **Prerequisite:** Stage 0 linear algebra + calculus; Python/NumPy (Stage 1)
- **Est. time:** ~30 hrs for Courses 2 + 4 combined (selective viewing)
- **Note:** 2022 content; CNN and optimization chapters remain fully current.

---

## 📌 Supplementary 2

### [Stanford CS231n — Notes + Assignments](https://cs231n.stanford.edu/)

- **Type:** Lecture notes + slides + assignments (self-study; no video required)
- **Cost:** Free
- **Math depth:** ⭐⭐⭐⭐☆ — The CS231n backpropagation notes are legendary; assignments demand implementing CNNs and RNNs from scratch in NumPy
- **Why this one:** The CS231n notes on backpropagation through computational graphs are the best *written* reference material available. Assignment 2 (vanilla RNN, LSTM from scratch in NumPy) provides the "derive by hand" experience for sequence models. **Video situation:** Recent lecture videos are restricted to enrolled Stanford students; 2017 YouTube lectures exist but are dated. The notes and slides are fully public — and are the higher-value component. 2024 Spring slides are on the course website and include transformer/ViT content.
- **Prerequisite:** Stage 3 Karpathy series complete (or in progress)
- **Est. time:** ~30 hrs (notes + Assignment 2)
- **Key links:**
  - Course notes: https://cs231n.github.io/
  - 2024 Slides: https://cs231n.stanford.edu/ (check "Assignments" tab)
  - Assignment 2 (RNN/LSTM in NumPy): linked from the course assignments page

---

## Orientation (Optional Pre-Stage 3)

### [MIT 6.S191 — Introduction to Deep Learning](http://introtodeeplearning.com)

- **Type:** Video lectures (~10 lectures, 60–75 min each) + Google Colab labs
- **Cost:** Free. YouTube: https://www.youtube.com/@MITDeepLearning
- **Math depth:** ⭐⭐⭐☆☆ — Rigorous enough for MIT standard but designed as an accelerated bootcamp overview
- **Why useful:** Annually updated (2024/2025 editions cover LLMs and generative AI); provides the big-picture map before diving deep with Karpathy. The Google Colab labs are immediately runnable. **Use as a 15-hour orientation sweep before starting Karpathy** — great for building a mental map.
- **Est. time:** ~15–20 hrs (lectures + labs)
- **Note:** Not a replacement for Karpathy — it skims optimization and regularization too quickly for deep mastery.

---

## References (Keep Bookmarked)

### [Deep Learning — Goodfellow, Bengio, Courville (2016)](https://www.deeplearningbook.org)
- **Cost:** Free online
- **Math depth:** ⭐⭐⭐⭐⭐ — The most mathematically rigorous free DL resource; full proofs for regularization and optimization
- **Usage:** Reference Chapters 6–8 for optimization theory (Adam derivation, momentum) when Ng feels too shallow. **Do NOT read cover-to-cover** — published 2016, does not cover transformers or modern architectures. Parts I–II are timeless; Part III is largely obsolete.

---

## ❌ Rejected Candidates

| Resource | Reason Rejected |
|----------|----------------|
| **fast.ai Practical Deep Learning (primary)** | Top-down style is the opposite of what's needed for math-rigorous stage. Part 1 math depth is minimal. Part 2 is useful but jumps to diffusion (too advanced for Stage 3 primary). Best as optional enrichment AFTER Karpathy. |
| **Andrew Ng DLS (primary)** | Good supplementary but surface-level math by comparison; "intuition-first" philosophy doesn't derive backprop the way Karpathy does. Selected courses (2 + 4) are kept as Supplementary 1 for CNN/optimization coverage. |
| **MIT 6.S191 (primary)** | Too compact — 10 hours covers what Karpathy's series covers in 60 hours. Excellent orientation but insufficient for mastery of any single topic. Kept as optional orientation. |
| **CS231n full course (primary)** | Videos restricted to enrolled students for recent editions; notes are publicly accessible but lack the hands-on code-along experience that makes Karpathy unique. Kept as Supplementary 2 for its legendary notes and assignments. |
