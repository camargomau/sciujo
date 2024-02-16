---
date: 2023-09-22
type: 🧠
tags:
  - MAC/S5/E1
---

**Topics:** [[Statistics]] - [[Probability]] - [[Standard Normal Distribution]]

---

_**(theorem)**_

Let $X_{1}, X_{2}, \dots, X_{n}$ be a [[Sequence|sequence]] of [[Independent and Identically Distributed Random Variables|iid]] [[Random Variable|random variables]] ([[Random Sample|random sample]]) such that $\forall X_{i}$:

$$
\begin{align*}
\mathbb{E}[X_{i}] &= \mu \\[0.5em]
\mathrm{Var}(X_{i}) &= \sigma^{2} \neq 0
\end{align*}
$$

Let $S_{n}$ be the sum of all of these random variables:

$$S_{n} = X_{1} + X_{2} + \dots + X_{n}$$

From the [[Properties of the Expected Value|properties of the expected value]] and those of [[Variance|variance]], it follows that $\mathbb{E}[S_{n}] = n\mu$ and $\mathrm{Var}(S_{n})=\sigma^{2}n$. Now, let:

$$
Z_{n} = \frac{S_{n}-n\mu}{\sigma\sqrt{n}}
$$

This is [[Random Variable Standarisation|standarisation]], so $\mathbb{E}[Z_{n}] = 0$ and $\mathrm{Var}(Z_{n})=1$.

The _central limit theorem_ tells us that when $n \to \infty$, the sequence $Z_{1}, Z_{2}, \dots, Z_{n}$ [[Limit of a Sequence|converges]] (in [[Probability Distribution|probability distribution]]) towards a [[Standard Normal Distribution|standard normal distribution]] $Z \sim \mathcal{N}(0,1)$.

# Usefulness

_**(observation)**_

The usefulness of the central limit theorem becomes evident when, given $Z \sim \mathcal{N}(0,1)$, we use it to affirm that:

$$
\lim_{ n \to \infty } \mathbb{P}\left( \frac{S_{n} - n\mu}{\sigma \sqrt{ n }} \leq z\right) = \mathbb{P}(Z \leq z)
$$

That is, the (standardised) sum of $n$ [[Independent and Identically Distributed Random Variables|iid]] random variables with _any_ distribution approaches a [[Standard Normal Distribution|standard normal distribution]] when $n \to \infty$.

This allows us to use a normal standard distribution to _approximate_ such a sum when $n$ is large enough.

_**(observation)**_

If we set $\overline{X}_{n} = \frac{S_{n}}{n}$, then we can write:

$$
\lim_{ n \to \infty } \mathbb{P}\left( \frac{\overline{X}_{n} - \mu} {\frac{\sigma}{\sqrt{n}}} \leq z \right) = \mathbb{P}(Z \leq z)
$$
