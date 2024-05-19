---
date: 2023-02-22
type: 🧠
tags:
  - MAC/S4/PB
---

**Topics:** [[Probability]]

---

_**(theorem)**_

Let $(B_i)_{i \in \mathbb{N}}$ be a [[Partition of a Sample Space|partition of a sample space]] and let $A$ be an [[Event|event]]. Then:

$$
\begin{align*}
\mathbb{P}(B_i \mid A) &= \frac{\mathbb{P}(A \mid B_i) \mathbb{P}(B_i)}{\mathbb{P}(A)} \\[0.5em]
&= \frac{\mathbb{P}(A \mid B_i) \mathbb{P}(B_i)}{\sum_{i \in \mathbb{N}} \mathbb{P}(A \mid B_i) \mathbb{P}(B_i)}
\end{align*}
$$

See [[Conditional Probability|conditional probability]]. The second equality follows after the [[Total Probability Formula|total probability formula]].

Basically, Bayes' theorem describes the [[Probability of an Event|probability of an event]] based on prior knowledge of conditions that might be related to the event.
