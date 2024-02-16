---
date: 2023-09-25
type: 🧠
tags:
  - MAC/S5/E1
---

**Topics:** [[Statistics]] - [[Normal Distribution]] [[Sampling Distribution]]

---

_**(theorem)**_

Let $X_{1}, \dots, X_{n}$ be [[Independent and Identically Distributed Random Variables|iid]] [[Random Variable|random variables]] ([[Random Sample|random sample]]) with a [[Normal Distribution|normal distribution]] that has an **unknown** [[Expected Value|expected value]], but a known [[Variance|variance]] $\sigma^{2}$.

Then:

$$
\frac{n-1}{\sigma ^{2}} S_{n-1}^{2} \sim \chi_{n-1}^{2}
$$

…where:

$$
S_{n-1}^{2} = \frac{\sum_{i=1}^n \left(x_{i} - \overline{X} \right)^{2}}{n-1}
$$

(i.e. [[Quasivariance|quasivariance]])

> [!tip]- Known Expected Value
> When we _do_ know the expected value of our random variables, [[Sampling Distribution of the Variance of a Normally Distributed Random Sample with an Unknown Expected Value|do something similar (this time with the traditional sample variance)]].
