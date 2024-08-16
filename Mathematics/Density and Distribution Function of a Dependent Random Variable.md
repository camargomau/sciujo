---
date: 2023-09-01
type: 🧠
tags:
  - MAC/4/PB
  - MAC/5/E1
---

**Topics:** [[Random Variable]] - [[Probability]]

---

# Integrating and Deriving

_**(theorem)**_

Let $X$ be an [[Absolutely Continuous Random Variable|absolutely continuous random variable]] with [[Density Function|density function]] $f_{X}(x)$. Let $\varphi : X \to \mathbb{R}$ be a [[Function|function]].

Let $Y = \varphi(X)$ be another random variable with [[Distribution Function|distribution function]] $F_{Y}(y) = \mathbb{P}(Y \leq y)$.

We can obtain $F_{Y}(y)$, $Y$'s distribution function, by integrating over the region on which $Y \leq y$. We can then obtain $f_{y}(y)$, $Y$'s density function, by deriving this distribution function.

> [!example]-
> Let $Y = 3X-1$ and let $f_{X}(x)$ be given by:
>
> $$
> f_{X}(x) =
> \begin{cases}
> 2x & \text{if } 0 \leq x \leq 1 \\
> 0 & \text{otherwise}
> \end{cases}
> $$
>
> We'll find $F_{Y}(y)$ by integrating:
>
> $$
> \begin{align*}
> F_{Y}(y) &= \mathbb{P}(Y \leq y) \\
> &= \mathbb{P}(3x - 1 \leq y) \\
> &= \mathbb{P}(3x \leq y  + 1) \\
> &= \mathbb{P}\left( x \leq \frac{y+1}{3} \right) \\
> &= \int_{0}^{\frac{y+1}{3}} f_{X}(x) \ dx \\
> &= \int_{0}^{\frac{y+1}{3}} 2x \ dx \\
> &= \frac{(y+1)^{2}}{9}
> \end{align*}
> $$
>
> Now, notice that $f_{X}(x)$ is $2x$ (what we integrated) when $0 \leq x \leq 1$. We'll find the corresponding values for this interval, in terms of $y$ by using $x = \frac{y+1}{3}$:
>
> - $\dfrac{y+1}{3} = 0 \implies y = -1 \implies F_{Y}(y) = 0$ when $y < -1$
> - $\dfrac{y+1}{3} = 1 \implies y = 2 \implies F_{Y}(y) = 1$ when $y > 2$
>
> Thus:
>
> $$
> F_{Y}(y) =
> \begin{cases}
> 0 & \text{if } y < -1 \\
> \dfrac{(y+1)^{2}}{9} & \text{if } -1 \leq y \leq 2 \\
> 1 & \text{if } y > 2
> \end{cases}
> $$
>
> Now, we can simply derivate to find the density function:
>
> $$
> f_{Y}(y) =
> \begin{cases}
> \frac{2}{9} (y+1) & \text{if } -1 \leq y \leq 2 \\
> 0 & \text{otherwise}
> \end{cases}
> $$

# Variable Change Theorem

_**(theorem)**_

Let $X$ be an absolutely continuous random variable with values in the interval $(a,b) \in \mathbb{R}$, and density function $f_{X}(x)$.

Let $\varphi(a,b) \to \mathbb{R}$ be a strictly increasing or decreasing continuous function with a [[Differentiable Function|differentiable]] [[Inverse Function|inverse]].

Then, the random variable $Y = \varphi(X)$ takes values in the interval $\varphi(a,b)$ and its density function is:

$$
f_{Y}(y) =
\begin{cases}
f_{X} \left( \varphi^{-1}(y) \right) \left| \frac{d\left(\varphi^{-1}(y)\right)}{dy} \right|  & \text{if } y \in \varphi(a,b) \\
0 & \text{otherwise}
\end{cases}
$$
