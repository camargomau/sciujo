---
date: 2023-09-27
type: 🧠
tags:
  - MAC/S5/E1
aliases:
  - MSE
---

**Topics:** [[Statistics]]

---

_**(definition)**_

Let $\hat{\theta}_{n}$ be an [[Estimator|estimator]] of parameter $\theta$.

The _mean squared error_ of $\hat{\theta}$ is the [[Expected Value|expected value]] of the square of the difference between $\hat{\theta}$ and $\theta$.

That is:

$$
\mathrm{MSE}(\hat{\theta}) = \mathbb{E} \left[ (\hat{\theta} - \theta)^{2} \right]
$$

_**(theorem)**_

We also have that:

$$
\mathrm{MSE}(\hat{\theta}) = \mathrm{Var}(\hat{\theta}) + \left( \mathrm{B}(\hat{\theta}) \right)^{2}
$$

(see [[Bias (Statistics)|bias]])

> [!quote]- Proof
> Notice that:
>
> $$
> \begin{align*}
> \mathrm{MSE}(\hat{\theta}_{n}) &= \mathbb{E}\left[ (\hat{\theta} - \theta)^{2} \right]  \\
> &= \mathbb{E}[\hat{\theta}^{2} - 2 \theta \hat{\theta} + \theta ^{2} ] \\
> &= \mathbb{E}[\hat{\theta}^{2}] - 2\theta \mathbb{E}[\hat{\theta}] + \theta^{2} \\
> &= \mathbb{E}[\hat{\theta}^{2}] - \left( \mathbb{E}[\hat{\theta}] \right)^{2} + \left( \mathbb{E}[\hat{\theta}] \right)^{2} - 2 \theta \mathbb{E}[\hat{ \theta}] + \theta ^{2} \\
> &= \mathrm{Var}(\hat{\theta}) + \left( \mathbb{E}[\hat{\theta}] - \theta \right)^{2} \\
> &= \mathrm{Var}(\hat{\theta}) - \left( \mathrm{B}(\hat{\theta}) \right)^{2}
> \end{align*}
> $$
