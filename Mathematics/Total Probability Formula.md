---
date: 2023-02-22
type: 🧠
tags:
  - MAC/4/PB
---

**Topics:** [[Partition of a Sample Space]] - [[Probability]] - [[Sample Space]]

---

_**(theorem)**_

Let $A \in \mathscr{F}$ (any event in the sample space; [[σ-Algebra|sigma-algebra]]) and let $(B_i)_{i \in \mathbb{N}}$ be a [[Partition of a Sample Space|partition of the sample space]]. Then:

$$
\begin{align*}
\mathbb{P}(A) &= \sum_{i \in \mathbb{N}} \mathbb{P}(A \mid B_i) \mathbb{P}(B_i) \\
&= \sum_{i \in \mathbb{N}} \mathbb{P}(A \cap B_i)
\end{align*}
$$

(see [[Conditional Probability|conditional probability]] and the third axiom for a [[Probability Measure|probability measure]])

We call this the _total probability formula_.
