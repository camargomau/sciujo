---
date: 2023-03-31
type: 🧠
tags:
  - MAC/S4/PB
---

**Topics:** [[Probability]]

---

# As a [[Moment]]

_**(definition)**_

Let $X$ be a [[Random Variable|random variable]].

The _variance_ of $X$, denoted $\mathrm{Var}(X)$, is defined as:

$$
\mathrm{Var}(X) := \mathbb{E}[(X - \mathbb{E}[X])^2]
$$

That is, the variance of $X$ is its [[Moment|second moment]].

_**(theorem)**_

Notice that $\mathrm{Var}(X)$ is also equivalent to:

$$
\mathrm{Var}(X) = \mathbb{E}[X^2] - (\mathbb{E}[X])^2
$$

# As a [[Measure of Dispersion]]

_**(definition)**_

Let $x_{1}, \dots, x_{n}$ be observations of a [[Random Variable|random variable]] $X$. The _variance_ of $X$ is:

$$
\mathrm{Var}(X) = \frac{1}{n} \sum_{i=1}^n \left(x_{i} - \overline{X} \right)^{2}
$$

…where $\overline{X}$ is the [[Mean|mean]] of $X$.

# Meaning

Variance quantifies how spread out the variable's mass is with respect to its mean.

Compare, for instance, the mass of the following two [[Population|populations]] with the same mean but different variances (blue has $\mathrm{Var}(X_{1}) = 100$; red has $\mathrm{Var}(X_{2}) = 2500$):

![[Variance-1.png]]

([courtesy of Wikimedia Commons](https://commons.wikimedia.org/wiki/File:Comparison_standard_deviations.svg))

# Properties

Let $X$ be a random variable whose [[Expected Value|expected value]] exists, and let $a, b \in \mathbb{R}$. Then:

1. $\mathrm{Var}(X) \geq 0$
2. $\mathrm{Var}(a) = 0$
3. $\mathrm{Var}(aX + b) = a^2\ \mathrm{Var}(X)$
