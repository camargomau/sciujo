---
date: 2023-04-21
type: 🧠
tags:
  - MAC/S4/PB
---

**Topics:** [[Probability]] - [[Bernoulli Distribution]]

---

_**(definition)**_

Let $X$ be a [[Random Variable|random variable]] that handles the repetition of [[Bernoulli Trial|Bernoulli trial]] ($X$: the number of successful trials). Let $n$ be the number of independent Bernoulli trials and $p$ be the probability of success.

In such a case, we say that $X$ has a _binomial distribution_ and write it as $X \sim \mathrm{Bin}(n,p)$.

> [!tip]- Single vs. Multiple Trials
> If $X$ handles **multiple** Bernoulli trials (of the same nature), then it has a binomial distribution.
>
> On the other hand, when it handles a **single** Bernoulli trial, it has a [[Bernoulli Distribution|Bernoulli distribution]].

# Density Function

_**(theorem)**_

The density function of an $X$ such that $X \sim \mathrm{Bin}(n,p)$ distribution is given by:

$$
f_{X}(x) =
\begin{cases}
\binom{n}{x} p^{x} (1-p)^{n-x} &\text{if } x \in \left\{ 0, \dots, n \right\} \\
0 &\text{otherwise}
\end{cases}
$$

# Expected Value

_**(theorem)**_

The [[Expected Value|expected value]] of such an $X$ is:

$$
\mathbb{E}[ X ] = np
$$

# Variance

_**(theorem)**_

The [[Variance|variance]] of such an $X$ is:

$$
\mathrm{Var}(X) = np(1-p)
$$

# Moment-Generating Function

_**(theorem)**_

Finally, the [[Moment-Generating Function|moment-generating function]] of such an $X$ is:

$$
M_X(t) = [(1-p) - pe^t]^n
$$
