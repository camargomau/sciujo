---
date: 2023-03-27
type: 🧠
tags:
  - MAC/4/PB
---

**Topics:** [[Probability]] - [[Random Variable]]

---

_**(definition)**_

Let $A$ be an [[Event|event]].

We define the _indicator random variable_ of $A$, denoted $\mathbb{1}_A$ as:

$$
X := \mathbb{1}_A
$$

…where $\mathbb{1}_{A}$ is the [[Indicator Function|indicator function]] for $A$:

$$
\mathbb{1}_A = \begin{cases}
1, &\text{ if } x \in A \\
0, &\text { if } x \notin A
\end{cases}
$$

# Density Function and Expected Value

The [[Density Function|density function]] of $X = \mathbb{1}_A$ an indicator random variable is always:

$$
f_X(x) =
\begin{cases*}
\mathbb{P}(A), \text{ if } x = 1 \\
\mathbb{P}(A^c), \text{ if } x = 0 \\
\end{cases*}
$$

Which tells us that its [[Expected Value|expected value]] is:

$$
\begin{align*}
\mathbb{E}[\mathbb{1}_A] = \mathbb{E}[X] &= 1 \mathbb{P}(A) + 0 \mathbb{P}(A^c) \\
&= \mathbb{P}(A)
\end{align*}
$$
