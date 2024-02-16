---
date: 2023-05-11
type: 🧠
tags:
  - MAC/S4/PB
aliases:
  - "rectangular distribution"
---

**Topics:** [[Probability]] - [[Distribution Function]]

---

_**(definition)**_

Let $X$ be an [[Absolutely Continuous Random Variable|absolutely continuous random variable]] such that $R_X = [a, b]$, where **all** intervals of a given length have the **same [[Probability of an Event|probability]]**.

In such a case, we say that $X$ has a _continuous uniform distribution_ (or _rectangular distribution_) and write $X \sim \mathrm{Unif}([a,b])$.

> [!tip]- Continuous Version
> Notice that this is just the [[Absolutely Continuous Random Variable|continuous]] version of the [[Discrete Uniform Distribution|discrete uniform distribution]].

# Density Function

_**(theorem)**_

The [[Density Function|density function]] of such an $X$ is given by:

$$
f_X(x) =
\begin{cases}
\frac{1}{b-a} &\text{if } a \leq x \leq b \\
0 &\text{otherwise}
\end{cases}
$$

# Distribution Function

_**(theorem)**_

Such an $X$'s [[Distribution Function|distribution function]] is:

$$
F_X(x) =
\begin{cases}
0 &\text{if } x < a \\
\frac{x-a}{b-a} &\text{if } a \leq x < b \\
1 &\text{if } x \geq b
\end{cases}
$$

# Expected Value

_**(theorem)**_

When it comes to the [[Expected Value|expected value]] of such an $X$, it is:

$$
\mathbb{E}[X] = \frac{a+b}{2}
$$

# Variance

_**(theorem)**_

As for the [[Variance|variance]] of such an $X$, it is:

$$
\mathrm{Var}(X) = \frac{(b-a)^2}{12}
$$

# Moment-Generating Function

_**(theorem)**_

The [[Moment-Generating Function|moment-generating function]] of such an $X$ is:

$$
M_X(t) = \frac{e^{tb} - e^{ta}}{t(b-a)}
$$
