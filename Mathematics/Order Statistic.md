---
date: 2023-09-13
type: 🧠
tags:
  - MAC/S5/E1
---

**Topics:** [[Statistics]]

---

_**(definition)**_

Let $X_{1}, \dots, X_{n}$ be a [[Random Sample|random sample]]. The variables:

$$
\begin{align*}
X_{(1)} &= \mathrm{min}\left\{ X_{1}, \dots, X_{n} \right\} \\
X_{(2)} &= \text{2nd }\mathrm{min}\left\{ X_{1}, \dots, X_{n} \right\} \\
&\vdots \\
X_{(n)} &= \mathrm{max}\left\{ X_{1}, \dots, X_{n} \right\} \\
\end{align*}
$$

…are called _order statistics_, where $X_{(i)}$ is the order statistic of order $i = 1, \dots, n$.

Note that these are just random variables defined as so, nothing more. Once we observe the sample and obtain every [[Random Variable Realisation|realisation]] $x_{i}$, then the [[Order Relation|order relation]] of the realisations is used to obtain, in turn, the realisations $x_{(i)}$ of the order statistics.

# Properties

_**(proposition)**_

Concerning the [[Density Function|density functions]] of order statistics:

1. $f_{X_{(1)}} (x) = nf(x) [1 - F(x)]^{n-1}$
2. $f_{X_{(n)}}(x) = nf(x) [F(x)]^{n-1}$
3. $f_{X_{(i)}}(x) = \binom{n}{i} i f(x) [F(x)]^{i-1} [1 - F(x)]^{n-i}$

…where $f(x)$ and $F(x)$ are the density and [[Distribution Function|distribution]] functions of every $X_{i}$ (remember that since they're a [[Random Sample|random sample]], they are [[Independent and Identically Distributed Random Variables|iid]]).

> [!warning]- What really are these?
> Do note that these are not the density functions of the random variable that corresponds to the $(i)$th random variable; that would just be $f(x)$. Rather, they are the density function of the random variable that is defined as:
>
> $$
> X_{i} = i\text{th min} \left\{ X_{1}, \dots, X_{n} \right\}
> $$
>
> To better understand what they are, know that ([[Distribution Function|distribution function]]):
>
> $$
> f_{X_{(i)}}(x) = \frac{d}{dx} \left[ F_{X_{(i)}}(x) \right]  = \frac{d}{dx} \left[ \mathbb{P}(X_{(i)} \leq x) \right]
> $$
>
> …where $\mathbb{P}(X_{(i)} \leq x)$ means $\mathbb{P}(\text{at least } i \text{ of the } n \text{ total } X_{i} \text{ are} \leq x)$.
