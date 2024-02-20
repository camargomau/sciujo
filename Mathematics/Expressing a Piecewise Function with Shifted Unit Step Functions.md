---
date: 2024-02-13
type: 🧠
tags:
  - MAC/6/ED2
---

**Topics:** [[Piecewise Function]]

---

_**(theorem)**_

Let $f(t)$ be a [[Piecewise Function|piecewise function]] of the following form:

$$
f(t) =
\begin{cases}
g(t) & \text{if } 0 \leq t < a \\
h(t) & \text{if } a \leq t < b \\
k(t) & \text{if } b \leq t
\end{cases}
$$

We can write such a function as follows, by using the [[Shifted Unit Step Function|shifted unit step function]] $U$:

$$
\begin{align*}
f(t) &= g(t) - g(t) U(t-a) + h(t) U(t-a) - h(t) U(t-b) + k(t) U(t-b) \\[0.5em]
&= g(t) + [h(t) - g(t)] U(t-a) + [k(t) - h(t)] U(t-b)
\end{align*}
$$
