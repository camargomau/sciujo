---
date: 2023-03-15
type: 🧠
tags:
  - MAC/4/PB
---

**Topics:** [[Probability Measure]] - [[Probability]]

---

_**(theorem)**_

Let $(A_n)_{n \geq 1}$ be a [[Increasing and Decreasing Sequence|non-decreasing]] [[Sequence|sequence]] of [[Event|events]]. Then:

$$
\mathbb{P}\left( \bigcup_{n=1}^\infty A_n \right) = \lim_{n \to \infty} \mathbb{P}(A_n)
$$

…where $\bigcup_{n=1}^\infty A_n = \lim_{n \to \infty} A_n$ (the [[Limit of a Sequence|limit of the sequence]]).

_**(theorem)**_

Let $(A_n)_{n \geq 1}$ be a non-increasing sequence of events. Then:

$$
\mathbb{P}\left( \bigcap_{n=1}^\infty A_n \right) = \lim_{n \to \infty} \mathbb{P}(A_n)
$$

…where $\bigcap_{n=1}^\infty A_n = \lim_{n \to \infty} A_n$.

_**(theorem)**_

Let $(A_n)_{n \geq 1}$ be a sequence of events that [[Limit of a Sequence|converges]] to an event $A$. Then:

$$
\mathbb{P}(A) = \lim_{n \to \infty} \mathbb{P}(A_n)
$$
