---
date: 2023-05-09
type: 🧠
tags:
  - MAC/4/PB
---

**Topics:** [[Probability]] - [[Distribution Function]]

---

_**(definition)**_

Let $X$ be a [[Random Variable|random variable]] that handles a single [[Bernoulli Trial|Bernoulli trial]] as follows:

$$
X(\omega) =
\begin{cases}
0 &\text{if } \omega = \text{failure} \\
1 &\text{if } \omega = \text{success}
\end{cases}
$$

Let $p$ be the [[Probability of an Event|probability]] of success.

In such a case, we say that $X$ has a _Bernoulli distribution_ and write $X \sim \mathrm{Ber}(p)$.

> [!tip]- Single vs. Multiple Trials
> If $X$ handles a **single** Bernoulli trial, then it has a Bernoulli distribution.
>
> On the other hand, when it handles **multiple** Bernoulli trials (of the same nature), it has a [[Binomial Distribution|binomial distribution]].

# Density Function

_**(theorem)**_

The [[Density Function|density function]] of such an $X$ is given by:

$$
f_X(x) =
\begin{cases}
p &\text{if } x = 1 \\
1-p &\text{if } x = 0 \\
0 &\text{otherwise}
\end{cases}
$$

# Distribution Function

_**(theorem)**_

As for the [[Distribution Function|distribution function]] of such an $X$:

$$
F_{X}(X) =
\begin{cases}
0 &\text{if }  x < 0 \\
1-p &\text{if } 0 \leq x < 1 \\
1 &\text{if } 1 \leq x
\end{cases}
$$

# Expected Value

_**(theorem)**_

When it comes to the [[Expected Value|expected value]] of such an $X$:

$$
\mathbb{E}[X] = p
$$

# Variance

_**(theorem)**_

For the [[Variance|variance]] of such an $X$:

$$
\mathrm{Var}(X) = p(1-p)
$$

# Moment-Generating Function

_**(theorem)**_

Such an $X$ has its [[Moment-Generating Function|moment-generating function]] given by:

$$
M_X(t) = e^t p + (1-p)
$$

# Characteristic Function

_**(theorem)**_

Finally, the [[Characteristic Function|characteristic function]] of $X$ is given by:

$$
\varphi_X(t) = e^{it} p + (1-p)
$$
