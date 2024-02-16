---
date: 2023-09-27
type: 🧠
tags:
  - MAC/S5/E1
---

**Topics:** [[Statistics]] - [[Estimator]]

---

_**(definition)**_

Let $\hat{\theta}_{n}$ be an [[Estimator|estimator]] for the parameter $\theta$, based on a [[Sample|sample]] of size $n$.

We say that $\hat{\theta}_{n}$ is _consistent_ if, for any $\varepsilon > 0$:

$$
\lim_{ n \to \infty } \mathbb{P}\left( | \hat{\theta}_{n} - \theta | > \varepsilon \right) = 0
$$

In other words, an estimator based on a sample of size $n$ is _consistent_ when the sequence $\hat{\theta}_{1}, \hat{\theta}_{2}, \dots, \hat{\theta}_{n}$ converges in [[Probability Distribution|probability distribution]] to $\theta$ as $n \to \infty$.

_**(proposition)**_

If $\hat{\theta}_{n}$ is an [[Estimator|estimator]] for $\theta$ and:

$$
\lim_{ n \to \infty } \mathbb{E}[\hat{\theta}_{n}] = \theta
$$

$$
\lim_{ n \to \infty } \mathrm{Var}(\hat{\theta}_{n}) = 0
$$

…then $\hat{\theta}_{n}$ is consistent.
