---
date: 2022-08-25
type: 🧠
tags:
  - MAC/S3/MN1
---

**Topics:** [[Numerical Analysis]] - [[Sequence]] - [[Limit of a Sequence]]

---

Let:

- $\{\beta_{n}\}_{n=1}^{\infty}$ be a [[Sequence|sequence]] that [[Limit of a Sequence|converges]] to $0$
- $\{\alpha_{n}\}_{n=1}^{\infty}$ be a sequence that converges to $\alpha \in \mathbb{R}$

We say that $\{\alpha_n\}$ converges to $\alpha$ with a _convergence speed_ of $O(\beta_{n})$ if:

$$
|\alpha_{n} - \alpha| \leq K|\beta_{n}|
$$

…where:

- $n$ is sufficiently big
- $\beta_{n}\neq 0$ for every $n$
- $K$ is a constant that's independent from $n$

We denote this with:

$$
\alpha_{n} = \alpha + O(\beta_{n})
$$
