---
date: 2023-03-27
type: 🧠
tags:
  - MAC/S4/PB
---

**Topics:** [[Probability]]

---

_**(definition)**_

Let $X$ be a real [[Random Variable|random variable]] defined on $(\Omega, \mathscr{F}, \mathbb{P})$.

The _expected value_ of a [[Random Variable|random variable]] $X$, denoted $\mathbb{E}[X]$, is defined as follows.

The expected value has [[Properties of the Expected Value|several properties]].

# Discrete Case

When $X$ is a [[Discrete Random Variable|discrete random variable]], we say that the expected value of $X$, $\mathbb{E}[X]$, exists if:

$$
\sum_{x \in R_X} |x| f_X(x) < \infty
$$

In such a case:

$$
\mathbb{E}[X] = \sum_{x \in R_X} x f_X(x)
$$

# Continuous Case

When $X$ is a [[Absolutely Continuous Random Variable|continuous random variable]], we say that the expected value of $X$, $\mathbb{E}[X]$, exists if:

$$
\int_{\mathbb{R}} |x| f_X(x)\ dx < \infty
$$

In such a case:

$$
\mathbb{E}[X] = \int_{\mathbb{R}} x f_X(x)\ dx
$$
