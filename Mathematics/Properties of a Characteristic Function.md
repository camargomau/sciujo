---
date: 2023-05-09
type: 🧠
tags:
  - MAC/S4/PB
---

**Topics:** [[Probability]] - [[Characteristic Function]]

---

_**(theorem)**_

Let $X$ be any [[Random Variable|random variable]]. Then, with respect to its [[Characteristic Function|characteristic function]] $\varphi_{X}(t)$. we have that:

1. The characteristic function of any random variable depends only on its [[Distribution Function|distribution]].

2. $\varphi_{X}(0) = \mathbb{E}[ e^{0} ] = 1$

3. The characteristic function takes values within the unit circle (i.e. $| \varphi_{X}(t) | \leq 1\ \forall t \in \mathbb{R}$

4. Let $Y$ be another random variable independent from $X$. Then $\varphi_{X+Y}(t) = \varphi_{X}(t) \varphi_{Y}(t)$

5. If $X$ and $Y$ are random variables such that $\varphi_{X}(t) = \varphi_{Y}(t)\ \forall t \in \mathbb{R}$, then $X$ and $Y$ have the same distribution.

6. The characteristic function is a [[Continuous Function|continuous function]].

# With Respect to Moments

_**(theorem)**_

Let $X$ be a random variable with an $n$th finite [[Moment|moment]]. Then:

1. The $n$th [[Derivative|derivative]] of $\varphi_{X}(t)$ exists and is continuous.
2. $$\begin{align*}
\left. \frac{d^n \varphi_{X}(t)}{dt^n} \right|_{t=0} &= i^n \mathbb{E}[ X^n ] \\[1em]
&\implies \\[1em]
\mathbb{E}[ X^n ] &= \frac{1}{i^n} \left. \frac{d^n \varphi_{X}(t)}{dt^n} \right|_{t=0}
\end{align*}
$$

# With Respect to Linear Functions

***(theorem)***

Let $a, b \in \mathbb{R}$ and $Y = aX+b$ with $X$ a [[Random Variable|random variable]]. Then:

$$
\varphi_{Y}(t) = e^{ibt} \varphi_{X}(at)
$$


# With Respect to Independent Random Variables

***(theorem)***

Let $X_{1}, \dots, X_{n}$ be [[Event Independence|independent]] random variables. Then:

$$
\varphi_{\sum \limits_{i=1}^{n} x_{i}}(t) = \prod_{k=1}^{n} \varphi_{X_k}(t)
$$

> [!warning]- The reciprocal is not true
> Note that the reciprocal is **not** true. That is:
>
> $$
> \begin{align*}
> \varphi_{X_1 + X_2}(t) &= \varphi_{X_1}(t) \varphi_{X_2}(t) \\[1em]
> &\centernot \implies \\[1em]
> X_1 \text{ and } X_2 &\text{ are independent}
> \end{align*}
> $$
