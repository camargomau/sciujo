---
date: 2024-02-13
type: 🧠
tags:
  - MAC/6/ED2
---

**Topics:** [[Laplace Transform]]

---

_**(theorems)**_

There are several theorems that prove to be fundamental when working with [[Laplace Transform|Laplace transforms]]:

$$
\begin{align*}
\mathcal{L}\{f(at)\} &= \frac{1}{a} F \left( \frac{s}{a} \right)  & \quad \text{(t. 9)} \\[1em]
\mathcal{L}\{f^{n}(t)\} &= s^{n} F(s) - s^{n-1} f(0) - \dots - f^{n-1} (0) & \quad \text{(t. 10)} \\[1em]
\mathcal{L}\{e^{at}f(t)\} &= F(s-a) & \quad \text{(t. 11)} \\[1em]
\mathcal{L}\{f(t-a)U(t-a)\} &= e^{-as} F(s) & \quad \text{(t. 12)} \\[1em]
\mathcal{L}\{t^{n}f(t)\} &= (-1)^{n} \frac{d^{n} F(s)}{ds^{n}}& \quad \text{(t. 13)} \\[1em]
\mathcal{L}\{f(t)g(t)\} &= F(s) G(s) & \quad \text{(t. 14)} \\[1em]
\end{align*}
$$

…where $U(t-a)$ is the [[Shifted Unit Step Function|shifted unit step function]]:

$$
U(t-a) =
\begin{cases}
0 & \text{if } 0 \leq t \leq a \\
1 & \text{if } t > a
\end{cases}
$$

> [!info]- Theorem Numbering
> The theorems are numbered according to my [[Ecuaciones Diferenciales II]] course.
