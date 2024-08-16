---
date: 2023-03-15
type: 🧠
tags:
  - MAC/4/PB
  - MAC/5/E1
---

**Topics:** [[Probability]]

---

_**(definition)**_

Let $X$ be a [[Random Variable|random variable]]. The _distribution function_ of $X$ is a [[Function|function]] $F_X : \mathbb{R} \to [0, 1]$ such that:

$$
F_X(x) = \mathbb{P}(X \leq x)
$$

Distribution functions have [[Properties of a Distribution Function|several properties]]. We can also define a distribution function at $x$ [[Distribution Function From the Left|from the left]].

# Developed Form

_**(theorem)**_

Notice that:

$$
F_X(y) = \mathbb{P}(X \leq y) = \sum_{x \in R_X}^y f_X(x)
$$

## Discrete

With this, we can write, for $X$ a [[Discrete Random Variable|discrete random variable]]:

$$
F_X(x) = \mathbb{P}(X \leq x) = \sum_{x_i \leq x} \mathbb{P}(X = x_i)
$$
## Continuous

For $X$ a [[Absolutely Continuous Random Variable|continuous random variable]]:

$$
F_X(x) = \mathbb{P}(X \leq x) = \int_{-\infty}^x f_X(t)\ dt
$$

# Well-Defined

_**(observation)**_

A distribution function is [[Well-Defined|well-defined]], since:

1. $$(-\infty, x] \in \mathcal{B}(\mathbb{R})$$
2. $$\{ X \in (-\infty, x] \} \in \mathscr{F}$$

3. $$\mathbb{P}(X \in (-\infty, x]) = \mathbb{P}(X \leq x) = F_X(x)$$

…with $\mathcal{B}(\mathbb{R})$ a [[Borel σ-Algebra|Borel σ-algebra]] and $\mathscr{F}$ a [[σ-Algebra|σ-algebra]].
