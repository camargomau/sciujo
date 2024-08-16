---
date: 2023-11-12
type: 🧠
tags:
  - MAC/5/E1
---

**Topics:** [[Estimator]] - [[Statistics]]

---

When trying to obtain [[Estimator|point estimators]], we can use the _maximum likelihood method_, which, given a [[Random Sample|random sample]] whose [[Probability Distribution|distribution]] depends on a [[Parameter (Statistics)|parameter]] $\theta$, consists of finding the value of $\theta$ that maximises the sample's [[Likelihood Function|likelihood function]].

This value of $\theta$ is called the _maximum likelihood estimator_ and we can use it to build an estimator for $\theta$.

# Procedure

Let $X_{1}, X_{2}, \dots, X_{n}$ be a random sample whose probability distribution depends on a parameter $\theta$. The _maximum likelihood method_ consists of maximising:

$$
\mathrm{L}(\theta \mid x) = \prod_{i=1}^{n} f(x_{i} \mid \theta)
$$

In other words, the method consists of finding the value of $\theta$ that maximises $\mathrm{L}(\theta \mid x)$. According to the theory behind [[Local Extremum|local extrema]], this is just finding the $\theta$ that satisfies:

$$
\begin{align*}
\frac{d}{d\theta} \left[ \mathrm{L}(\theta \mid x) \right] &= 0 \\[1em]
\frac{d^{2}}{d\theta^{2}} \left[ \mathrm{L}(\theta \mid x) \right] &< 0
\end{align*}
$$

## Natural Logarithm

Sometimes, it might be a good idea to instead maximise:

$$
\ln \left[ \mathrm{L}(\theta \mid x) \right] 
$$
