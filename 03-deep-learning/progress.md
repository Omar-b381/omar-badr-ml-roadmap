# Stage 3 — Progress Tracker

---

## Optional: MIT 6.S191 Orientation (~15–20 hrs)

- [ ] Lecture 1: Intro to Deep Learning
- [ ] Lecture 2: Recurrent Neural Networks and Transformers
- [ ] Lecture 3: CNNs
- [ ] Lecture 4: Deep Generative Models
- [ ] Colab Lab 1: Intro to TensorFlow + basic NN
- [ ] Colab Lab 2: CNNs and data augmentation

**MIT 6.S191 Orientation COMPLETE:** ⬜ — Date: ___

---

## Karpathy — Neural Networks: Zero to Hero (PRIMARY)

### Video 1: Backprop from scratch — building `micrograd` ⭐ (Most Important)
- [ ] Watch full video (~2.5 hrs)
- [ ] Implement `Value` class with `__add__`, `__mul__`, `__pow__`
- [ ] Implement backward pass for each operation
- [ ] Build computational graph manually for a simple 2-layer network
- [ ] Implement `backprop()` via topological sort
- [ ] Verify gradients match numerical gradient check
- [ ] Connect to PyTorch autograd — verify same results

**Video 1 COMPLETE:** ⬜ — Date: ___

### Video 2: MLP — building makemore (bigram model → MLP)
- [ ] Watch full video (~1 hr)
- [ ] Implement bigram language model in PyTorch
- [ ] Build MLP for character-level name generation
- [ ] Implement manual training loop (no `nn.Module`)

**Video 2 COMPLETE:** ⬜ — Date: ___

### Video 3: Activations & Gradients — deep dive
- [ ] Watch full video (~1.5 hrs)
- [ ] Visualize activation and gradient distributions during training
- [ ] Understand dead ReLU neurons and gradient saturation
- [ ] Implement Xavier initialization and understand why it works

**Video 3 COMPLETE:** ⬜ — Date: ___

### Video 4: BatchNorm — from scratch
- [ ] Watch full video (~1 hr)
- [ ] Implement BatchNorm forward and backward pass manually
- [ ] Understand the gradient flow through BatchNorm
- [ ] Understand why BatchNorm helps optimization

**Video 4 COMPLETE:** ⬜ — Date: ___

### Videos 5–6: WaveNet / makemore architecture
- [ ] Watch Video 5 (~1 hr)
- [ ] Watch Video 6 (~1 hr)
- [ ] Implement the WaveNet-style dilated CNN architecture
- [ ] Understand hierarchical feature learning

**Videos 5–6 COMPLETE:** ⬜ — Date: ___

### Video 7: Let's build GPT from scratch (Bridge to Stage 4) ⭐
- [ ] Watch full video (~2 hrs)
- [ ] Implement self-attention from scratch
- [ ] Implement multi-head attention
- [ ] Implement positional encoding
- [ ] Assemble the full decoder-only transformer
- [ ] Train on Tiny Shakespeare dataset

**Video 7 COMPLETE:** ⬜ — Date: ___

**Karpathy Zero to Hero COMPLETE:** ⬜ — Date: ___

---

## Andrew Ng DLS — Courses 2 & 4 (SUPPLEMENTARY 1)

### Course 2: Improving Deep Neural Networks (Hyperparameter tuning, Optimization)
- [ ] Week 1: Regularization (dropout, L2, early stopping)
- [ ] Week 1: Setting up optimization (bias/variance trade-off, weight initialization)
- [ ] Week 2: Optimization algorithms (mini-batch GD, momentum, RMSprop, Adam)
- [ ] Week 3: Tuning, batch normalization, softmax
- [ ] Programming Assignment: Optimization Methods (implement Adam, RMSprop from scratch)
- [ ] Programming Assignment: Regularization

**Course 2 COMPLETE:** ⬜ — Date: ___

### Course 4: Convolutional Neural Networks
- [ ] Week 1: Foundations of CNNs (convolution operation, pooling)
- [ ] Week 2: Deep CNNs (ResNets, inception)
- [ ] Week 3: Object detection (YOLO, anchors)
- [ ] Week 4: Face recognition, neural style transfer
- [ ] Programming Assignment: Build CNN from scratch in NumPy
- [ ] Programming Assignment: Implement ResNet

**Course 4 COMPLETE:** ⬜ — Date: ___

---

## CS231n Notes + Assignment 2 (SUPPLEMENTARY 2)

### Lecture Notes (Read; no videos required)
- [ ] [Linear classification (SVM, Softmax)](https://cs231n.github.io/linear-classify/)
- [ ] [Optimization](https://cs231n.github.io/optimization-1/)
- [ ] [Backpropagation and computational graphs](https://cs231n.github.io/optimization-2/) ⭐
- [ ] [Neural networks Part 1 (architectures)](https://cs231n.github.io/neural-networks-1/)
- [ ] [Neural networks Part 2 (data processing, regularization)](https://cs231n.github.io/neural-networks-2/)
- [ ] [Neural networks Part 3 (learning, evaluation)](https://cs231n.github.io/neural-networks-3/)
- [ ] [Convolutional networks](https://cs231n.github.io/convolutional-networks/)
- [ ] [RNNs (with BPTT derivation)](https://cs231n.github.io/rnn/) ⭐

### Assignment 2 (Implement from scratch)
- [ ] Q3: Vanilla RNN implementation in NumPy (including BPTT)
- [ ] Q4: LSTM implementation in NumPy
- [ ] Q5: Network visualization (optional)

**CS231n Notes + Assignment 2 COMPLETE:** ⬜ — Date: ___

---

## ✅ Stage 3 Sign-Off

- [ ] Can I build a scalar-valued autograd engine in pure Python from scratch?
- [ ] Can I manually compute the gradient of a 2-layer network by hand?
- [ ] Can I implement BatchNorm forward and backward pass from scratch?
- [ ] Can I implement a vanilla RNN in NumPy with BPTT?
- [ ] Can I implement the Adam optimizer from scratch?
- [ ] Can I explain what dropout does to the computational graph?
- [ ] Can I build a CNN from scratch (NumPy conv operation)?

**Stage 3 COMPLETE → Ready for Stage 4:** ⬜ — Date: ___
