---
date: 2024-02-19
type: 🧠
tags:
  - MAC/6/ED2
---

**Topics:** [[Laplace Transform]]

---

Concerning [[Laplace Transform|Laplace transforms]], we can guarantee their existence by means of the consequences of the following theorems. 

_**(theorem, 8)**_

Note that, as $t$ increases, the growth of the [[Complex Number Module|module]] of the function $f(t)$ is not greater than that of an [[Exponential Function|exponential function]]. That is, there exists $M > 0$ and $s_{0} \geq 0$ such that, for every value of $t$:

$$
\left| f(t) \right| < Me^{s_{0}t}
$$

We call $s_{0}$ the _growth exponent_ of the function $f(t)$. This condition guarantees the existence of the Laplace transform. 

_**(theorem)**_

If $f(t)$ is [[Piecewise Continuous|piecewise continuous]] in every finite set $0 < t < M$ of exponential order $s_{0}$ for $t > M$, then the Laplace transform $F(s)$ exists as long as $s_0 > 0$.
