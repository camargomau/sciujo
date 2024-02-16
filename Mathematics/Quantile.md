---
date: 2023-08-21
type: 🧠
tags:
  - MAC/S5/E1
---

**Topics:** [[Statistics]]

---

_**(definition)**_

Let $x_{1}, \dots, x_{n}$ be observations of a [[Random Variable|random variable]] $X$ and let $p \in (0, 1)$.

A _quantile_ to the $100p\%$ is the value _c_ that satisfies the following two conditions:

1. $$\frac{\left| \left\{ x_{i} \mid x_{i} \leq c \right\} \right|}{n} \geq p$$
2. $$\frac{\left| \left\{ x_{i} \mid x_{i} \geq c \right\} \right|}{n} \geq 1 - p$$

…where $|S|$ denotes the [[Cardinality|cardinality]] of $S$.

# Meaning

A is basically the value up to which the $100p\%$ of the variable's mass is accumulated.

See, for instance, the location of the quartiles ($25\%, 50\%, 75\%$) of a [[Normal Distribution|normal distribution]]:

![[Quantile-1.png]]

([courtesy of Wikimedia Commons](https://commons.wikimedia.org/wiki/File:Iqr_with_quantile.png))

# Particular Cases

- _Decile_: if $p = \left\{ 0.1, \dots, 0.9 \right\}$
- _Quartile_: if $p = \left\{ 0.25, 0.50, 0.75 \right\}$
- _Percentile_: if $p = \left\{ 0.01, 0.02, \dots, 0.99 \right\}$

Notice that the second quartile is the [[Median|median]].
