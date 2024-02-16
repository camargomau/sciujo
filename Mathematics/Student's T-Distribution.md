---
date: 2023-09-18
type: 🧠
tags:
  - MAC/S5/E1
---

**Topics:** [[Probability]] - [[Standard Normal Distribution]] - [[Chi-Squared Distribution]]

---

_**(definition)**_

Let $X$ and $Y$ be [[Event Independence|independent]] [[Random Variable|random variable]] such that $X \sim \mathcal{N}(0,1)$ and $Y \sim \chi_{(n)}^2$. Let:

$$
W = \frac{X}{\sqrt{ \frac{Y}{n} }}
$$

In such a case, we say that $W$ has a _Student's t-distribution_ with $n$ degrees of freedom.

# Expected Value and Variance

_**(theorem)**_

A random variable $W$ with a Student's t-distribution has an [[Expected Value|expected value]] and [[Variance|variance]] of:

$$
\mathbb{E}[W] = 0
$$

$$
Var(W) = \frac{n}{n-2}
$$
