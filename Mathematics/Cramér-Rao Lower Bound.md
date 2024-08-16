---
date: 2023-10-04
type: 🧠
tags:
  - MAC/5/E1
---

**Topics:** [[Statistics]]

---

_**(theorem)**_

Let $X_{1}, \dots, X_{n} \sim f(x \mid \theta)$, with $\theta \in \Theta$ (i.e. a [[Parameter (Statistics)|parameter]] in a [[Parameter Space|parameter space]]).

Let $T$ be an [[Estimator|estimator]] of $\theta$. Then:

$$
\mathrm{Var}(T) \geq \frac{1}{n \mathbb{E}\left[ \left( \frac{d \ln \left( f(x \mid \theta) \right) }{d \theta} \right)^{2} \right]} := \mathrm{CRLB}(\theta)
$$

In other words, the _Cramér-Rao lower bound_ ($\mathrm{CRLB}(\theta)$) provides a [[Upper and Lower Bounds|lower bound]] for $T$'s [[Variance|variance]].
