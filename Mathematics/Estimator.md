---
date: 2023-10-13
type: 🧠
tags:
  - MAC/5/E1
---

**Topics:** [[Statistics]] - [[Sample Statistic]]

---

_**(definition)**_

An _estimator_ is a [[Sample Statistic|sample statistic]] that aims to _estimate_ a given [[Parameter (Statistics)|parameter]] of the [[Random Sample|random sample]] at hand.

More formally, given a [[Random Variable|random variable]] $X$ and its corresponding [[Random Sample|random sample]] $X_{1}, X_{2}, \dots, X_{n}$ characterised by a parameter $\theta$, an _estimator_ $\hat{\theta}$ is a function $\hat{\theta}(X) = f(X_{1}, X_{2}, \dots, X_{n})$ that returns an approximation of $\theta$.

# Quality

Of course, not all estimators for a same parameter are the same.

For instance, there can be [[Unbiased Estimator|unbiased]], [[Asymptotically Unbiased Estimator|asymptotically unbiased]], [[Efficient Estimator|efficient]], [[Consistent Estimator|consistent]] and [[Uniformly Minimum-Variance Unbiased Estimator|uniformly minimum-variance unbiased (UMVUE)]] estimators, to name just a few.

We generally prefer unbiased, efficient and minimum-variance estimators, since they tend to give a better approximation to the actual value of the parameter.
