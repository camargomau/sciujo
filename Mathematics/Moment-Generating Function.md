---
date: 2023-04-10
type: 🧠
tags:
  - MAC/S4/PB
---

**Topics:** [[Probability]] - [[Moment]]

---

_**(definition)**_

$$
M_X(t) := \mathbb{E}\left[ e^{tX} \right]
$$

…with $t \in (-h, h)$ given $h > 0$. This implies that $M_X(t)$ is differentiable at $t = 0$.

Do note that **not all** distributions of probability have a moment-generating function.

Moment-generating functions have [[Properties of a Moment-Generating Function|several properties]].

# Discrete Case

_**(theorem, from [[Law of the Unconscious Statistician|the law of the unconscious statistician]])**_

When $X$ is a [[Discrete Random Variable|discrete random variable]]. then:

$$
M_X(t) = \sum_{x \in R_X} e^{tx} f_X(x)
$$

# Continuous Case

_**(theorem, from [[Law of the Unconscious Statistician|the law of the unconscious statistician]])**_

When $X$ is an [[Absolutely Continuous Random Variable|absolutely continuous random variable]], then:

$$
M_X(t) = \int_\mathbb{R} e^{tx} f_X(x)\ dx
$$

# $n$th moment

_**(theorem)**_

In general, we have that:

$$
E[X^n] = \left. \frac{d^n M_X(t)}{dt^n} \right|_{t=0}
$$

That is, the $n$th (non-central) [[Moment|moment]] of $X$ is given by the $n$th derivative of $M_X(t)$ evaluated at $t = 0$.
