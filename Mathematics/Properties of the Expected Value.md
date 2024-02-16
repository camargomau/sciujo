---
date: 2023-03-31
type: 🧠
tags:
  - MAC/S4/PB
---

**Topics:** [[Expected Value]] - [[Probability]]

---

_**(theorem)**_

Let $X$ be a [[Random Variable|random variable]] and $a, b \in \mathbb{R}$. Then, the [[Expected Value|expected value]] of $X$ has the following properties

1. If $\mathbb{P}(X \geq 0) = 1$ ($X$ always positive), then $\mathbb{E}[X] \geq 0$.
2. If $X = a$ ($X$ is constant), then $\mathbb{E}[X] = a$
3. $\mathbb{E}[aX + b] = a \mathbb{E}[X] + b$
4. If $\mathbb{E}[X]$ exists, then $|\mathbb{E}[X]| \leq \mathbb{E}[|X|]$
5. If $g$ and $h$ are [[Function|functions]] such that $g(x)$ and $h(x)$ are random variables whose values exist, if $g(x) \leq h(x)\ \forall x$, then $\mathbb{E}[g(x)] \leq \mathbb{E}[h(x)]$
