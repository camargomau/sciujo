---
date: 2023-05-11
type: 🧠
tags:
  - MAC/S4/PB
---

**Topics:** [[Probability]] - [[Distribution Function]]

---

_**(definition)**_

Let $X$ be an [[Absolutely Continuous Random Variable|absolutely continuous random variable]].

We say that $X$ has a _normal distribution_ (or _Gaussian distribution_) if its [[Density Function|density function]] is:

$$
f_X(x) =
\begin{dcases}
\frac{1}{\sigma \sqrt{2 \pi}}e^{-\frac{(x - \mu)^{2}}{2 \sigma^{2}}} &\text{if } x \in \mathbb{R} \\
0 &\text{otherwise}
\end{dcases}
$$

…and write $X \sim \mathcal{N}(\mu, \sigma^{2})$.

> [!info]- Applications
> Random variables with normal distributions help us model many natural, social and psychological phenomena, including, but not limited to:
>
> - Height
> - Effects of a drug
> - [[Intelligence Quotient|Intelligence quotient]]
> - Noise level in telecommunications

In particular, the random variable $X$ such that $X \sim \mathcal{N}(0, 1)$ is of special importance: its distribution is called the **[[Standard Normal Distribution|standard normal distribution]]**.

# Expected Value and Variance

Notice that this probability distribution depends on two parameters: $\mu$ and $\sigma^{2}$.

_**(theorem)**_

The [[Expected Value|expected value]] of an $X$ with a normal distribution is simply and elegantly:

$$
\mathbb{E}[X] = \mu
$$

_**(theorem)**_

The [[Variance|variance]] of an $X$ with a normal distribution is simply and elegantly:

$$
\mathrm{Var}(X) = \sigma^{2}
$$

Indeed, we use these two values as parameters since:

- $\mu$ provides the value around which most of the mass concentrates. It is a _localisation_ parameter: if we change it, the curve moves horizontally, but it stays otherwise the same.

- $\sigma$ provides the distribution's [[Standard Deviation|standard deviation]] (i.e. a measure of how disperse the mass is around $\mu$). It is a _dispersion_ parameter: if we change it, the concentration of the mass changes, but the curve stays in the same location.

# Examples

A few examples of the density distribution graphs of various normal distributions with different parameters:

![[Normal Distribution-1.png|450]]

Notice how, effectively, the mass concentrates around $\mu$ and $\sigma$ provides a dispersion measure, as mentioned before.

The red curve is the _standard_ normal distribution.
