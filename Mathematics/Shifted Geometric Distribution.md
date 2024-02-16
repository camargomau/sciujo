---
date: 2023-05-10
type: 🧠
tags:
  - MAC/S4/PB
---

**Topics:** [[Probability]] - [[Distribution Function]]

---

_**(definition)**_

Let $X$ be a [[Discrete Random Variable|discrete random variable]] that handles the repetition of a [[Bernoulli Trial|Bernoulli trial]] until success is achieved. Let $p$ be the [[Probability of an Event|probability]] of success.

More specifically, let $X$ handle the **number of trials** needed to get one success (i.e. $R_X = \{1, 2, 3, \dots \}$).

For such an $X$, we say that it has a _**shifted** geometric distribution_ and write $X \sim \mathrm{Geo}(p)$.

> [!info]- Non-Shifted Geometric Distribution
> When $X$ handles the **number of failures** before the first success (i.e. $R_X = \{0, 1, 2, \dots \}$), we say that it has a _geometric distribution_ (non-shifted). See [[Geometric Distribution|this note]] for more details on that distribution.
>
> Both of these distributions are commonly simply called _geometric_, with no other differentiating term. Which of these two distributions is being talked about is a matter of context and/or convention.
>
> There is a convention to refer to the one that counts the trials as the _shifted geometric distribution_, and that's what I use in all of my notes.

# Density Function

_**(theorem)**_

Such an $X$ has the following [[Density Function|density function]]:

$$
f_X(x) =
\begin{cases}
(1-p)^{x-1} p &\text{if } x = 1, 2, 3, \dots \\
0 &\text{otherwise}
\end{cases}
$$

# Expected Value

_**(theorem)**_

When it comes to the [[Expected Value|expected value]] of such an $X$, it is:

$$
\mathbb{E}[X] = \frac{1}{p}
$$

# Variance

_**(theorem)**_

As for the [[Variance|variance]] of such an $X$:

$$
\mathrm{Var}(X) = \frac{1-p}{p^{2}}
$$

# Moment-Generating Function

_**(theorem)**_

Finally, such an $X$ has the following moment-generating function:

$$
M_X(t) = \frac{pe^t}{1-(1-p)e^t}
$$
