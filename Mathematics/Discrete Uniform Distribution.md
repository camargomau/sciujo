---
date: 2023-05-09
type: 🧠
tags:
  - MAC/S4/PB
---

**Topics:** [[Probability]] - [[Distribution Function]]

---

_**(definition)**_

Let $X$ be a [[Discrete Random Variable|discrete]] [[Random Variable|random variable]] such that its range is $R_X = \{ x_1, \dots, x_n \}$ and the occurrence of every one of these elements is equally as probable.

That is, let $X$ such that its [[Distribution Function|distribution function]] is:

$$
f_X(x) =
\begin{cases}
\frac{1}{n} &\text{if } x \in \{ x_1, \dots, x_n \} \\
0 &\text{otherwise}
\end{cases}
$$

In such a case, we say that $X$ has a _uniform distribution_. We denote this with $X \sim \mathrm{Unif} (\{ x_1, \dots, x_n \})$

# Expected Value

_**(theorem)**_

The [[Expected Value|expected value]] of such an $X$ is given by:

$$
\mathbb{E}[X] = \frac{1}{n} \sum_{x \in R_X} x
$$

# Variance

_**(theorem)**_

The [[Variance|variance]] of such an $X$ is given by:

$$
\mathrm{Var}(X) = \frac{1}{n} \sum_{x \in R_X} (x - \mathbb{E}[X])^2
$$
