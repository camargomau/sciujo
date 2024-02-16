---
date: 2023-05-11
type: 🧠
tags:
  - MAC/S4/PB
---

**Topics:** [[Probability]] - [[Distribution Function]] - [[Normal Distribution]]

---

_**(definition)**_

The _standard normal distribution_, commonly denoted $Z$, is a [[Normal Distribution|normal distribution]] such that $\mu = 0$ and $\sigma^2 = 1$.

In other words, if $X$ a [[Random Variable|random variable]] is such that $X \sim \mathcal{N}(0,1)$, we say that it follows a _standard normal distribution_, and commonly denote it $Z$.

![[Standard Normal Distribution-1.png]]

# Standardisation

The values of $Z$'s [[Distribution Function|distribution function]] are well known and can be easily found in tables. We can use these tables to facilitate our calculations with any other normal distribution $X \sim \mathcal{N}(\mu, \sigma^2)$, since we can standardise $X$ as follows:

$$
Z = \frac{X - \mu}{\sigma}
$$

# Properties

Let $Z$ be a [[Random Variable|random variable]] with a standard normal distribution. Then:

- The [[Mean|mean]], the [[Median|median]] and the [[Mode|mode]] of $Z$ are all equal to $\mu$.
- $68\%$ of the observations fall in the interval $[\mu - \sigma, \mu + \sigma]$.
- $95\%$ of the observations fall in the interval $[\mu - 2 \sigma, \mu + 2 \sigma]$.
- $99.7\%$ of the observations fall in the interval $[\mu - 3 \sigma, \mu + 3 \sigma]$.
