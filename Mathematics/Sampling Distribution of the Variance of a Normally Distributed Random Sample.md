---
date: 2023-09-25
type: 🧠
tags:
  - MAC/5/E1
---

**Topics:** [[Statistics]] - [[Variance]] - [[Sampling Distribution]]

---

_**(theorem)**_

Let $X_{1}, \dots, X_{n}$ be [[Independent and Identically Distributed Random Variables|iid]] [[Random Variable|random variables]] ([[Random Sample|random sample]]) with a [[Normal Distribution|normal distribution]], [[Expected Value|expected value]] $\mu$ and [[Variance|variance]] $\sigma^{2}$.

Then:

$$
\frac{nS_{n}^{2}}{\sigma^{2}} \sim \chi_{n}^{2}
$$

…where:

$$
S_{n}^{2} = \frac{\sum_{i=1}^n (x_{i} - \mu)^{2}}{n}
$$

That is, $S_{n}^{2}$ is the sample variance.

> [!tip]- Unknown Expected Value
> When we don't know the expected value of our random variables, [[Sampling Distribution of the Variance of a Normally Distributed Random Sample with an Unknown Expected Value|do something similar (albeit with a slightly different sample variance)]].
