---
date: 2023-03-31
type: 🧠
tags:
  - MAC/4/PB
---

**Topics:** [[Probability]] - [[Expected Value]]

---

# As an [[Expected Value]]

## Central

_**(definition)**_

Let $X$ be a [[Random Variable|random variable]] and let $\mathbb{E}[X]$ be its [[Expected Value|expected value]].

We say that the _central moment of $X$ of order $r$_ is:

$$
m_{r} = \mathbb{E}[(X - \mathbb{E}[X])^r]
$$

The second moment is better known as [[Variance|variance]]; the third is known as [[Skewness|skewness]]; the fourth is known as [[Kurtosis|kurtosis]].

> [!question]- Developed Form
> Recall that, from the [[Law of the Unconscious Statistician|law of the unconscious statistician]], for $X$ a [[Discrete Random Variable|discrete random variable]] such that $\mathbb{E}[X] = \mu$:
>
> $$
> \mathbb{E}[(X - \mathbb{E}[X])^{r}] = \sum_{R_{X^r}} (x - \mu)^{k} f_X(x)
> $$
>
> And for a similar $X$, an [[Absolutely Continuous Random Variable|absolutely continuous random variable]]:
>
> $$
> \mathbb{E}[(X - \mathbb{E}[X])^{r}] = \int_\mathbb{R} (x - \mu)^{k} f_X(x)\ dx
> $$

## Non-Central

_**(theorem)**_

We say that the _(non-central) moment of $X$ of order $r$_ is:

$$
m'_{r} = \mathbb{E}[X^r]
$$

> [!tip]- The Expected Values of the Powers of $X$
> Notice that the expected value of $X$ is its first non-central moment.
>
> More generally, notice that the non-central moments of $X$ are the expected values of the powers of $X$.

> [!question]- Developed Form
> Recall that, from the [[Law of the Unconscious Statistician|law of the unconscious statistician]], for $X$ a [[Discrete Random Variable|discrete random variable]]:
>
> $$
> \mathbb{E}[X^r] = \sum_{R_{X^r}} x^r f_X(x)
> $$
>
> And for $X$ an [[Absolutely Continuous Random Variable|absolutely continuous random variable]]:
>
> $$
> \mathbb{E}[X^r] = \int_\mathbb{R} x^r f_X(x)\ dx
> $$

_**(observation)**_

Notice that when $\mathbb{E}[X] = 0$, then $m_{k} = m'_{k}\ \forall k \in \mathbb{N}$.

## Properties

_**(theorem)**_

Let $X$ be a random variable with a moment of finite order $n$. Then:

- $\mathbb{E}[X^r]$ exists for $r \leq n$
- $\mathbb{E}[(X-a)^r]$ exists for each $r \leq n$ and for every $a \in \mathbb{R}$

# As a [[Measure of Shape]]

## Central

_**(definition)**_

Let $x_{1}, \dots, x_{n}$ be observations of a [[Variable (Statistics)|variable]] $X$.

The $k$th _central_ moment of $X$ (i.e. of order $k$) is defined as:

$$
m_{k}(X) = \frac{1}{n} \sum_{i=1}^n (x_{i} - \overline{X})^k
$$

…where $\overline{X}$ denotes the [[Mean|mean]] of $X$.

## Non-Central

_**(definition)**_

On the other hand, the $k$th (non-central) moment of $X$ is:

$$
m_{k}'(X) = \frac{1}{n} \sum_{i=0}^n x_{i}^k
$$
