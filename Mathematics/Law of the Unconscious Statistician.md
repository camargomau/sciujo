---
date: 2023-03-31
type: 🧠
tags:
  - MAC/4/PB
---

**Topics:** [[Probability]] - [[Expected Value]]

_**(theorem)**_

Let $X$ be a [[Random Variable|random variable]] and let $g : \mathbb{R} \to \mathbb{R}$ be a [[Function|function]] such that $Y = g(x)$ is also a random variable.

If we wanted to calculate $\mathbb{E}[Y]$, the [[Expected Value|expected value]] of $Y$, we would have to first find $f_Y$ (its [[Density Function|density function]]). There is, however, a simpler way to calculate it, called the _law of the unconscious statistician_.

> [!example]-
> Let $X$ be a discrete random variable where $\mathbb{E}[X] = 0$ whose density function is defined as:
>
> $$
> f_X(x) = \begin{cases}
> \frac{1}{9}, &\text{ if } x \in \{-4, -3, -2, -1, 0, 1, 2, 3, 4\} \\
> 0, &\text{ otherwise}
> \end{cases}
> $$
>
> Let $Z = (X - \mathbb{E}[X])^2 = X^2$. What's $\mathbb{E}[Z]$?
>
> ---
>
> **Normal way:**
>
> We can calculate $\mathbb{E}[Z]$ in the normal way. We first determine its density function:
>
> $$
> f_Z(z) = \begin{cases} \tfrac{1}{9}, \text{ if } z = 0 \\ \tfrac{2}{9}, \text{ if } z = 1, 4, 9, 16 \\ 0, \text{ otherwise} \end{cases}
> $$
>
> Then we use the definition of an expected value:
>
> $$
> \begin{align*}
> \mathbb{E}[Z] &= \sum_{x = 0}^{16} z\ \mathbb{P}(Z = z) \\
> &= (0) \frac{1}{9} + (1) \frac{2}{9} + (4) \frac{2}{9} + (9) \frac{2}{9} + (16) \frac{2}{9} \\
> &= \frac{60}{9}
> \end{align*}
> $$
>
> ---
>
> **With the law of the unconscious statistician:**
>
> However, it is much easier if we just use the law of the unconscious statistician. Since $X$ is a discrete random variable, then:
>
> $$
> \begin{align*}
> \mathbb{E}[Z] = \mathbb{E}[X^2] &= \sum_{x = -4}^4 x^2\ \mathbb{P}(X = x) \\
> &= (-4)^2 \frac{1}{9} + (-3)^2 \frac{1}{9} + (-2)^2 \frac{1}{9} + (-1)^2 \frac{1}{9} \\
> &\quad +\ 0^2 \frac{1}{9} + 1^2 \frac{1}{9} + 2^2 \frac{1}{9} + 3^2 \frac{1}{9} + 4^2 \frac{1}{9} \\
> &= \frac{60}{9}
> \end{align*}
> $$

# Discrete Case

If $X$ is a [[Discrete Random Variable|discrete random variable]], then:

$$
\mathbb{E}[Y] = \mathbb{E}[g(x)] = \sum_{x \in R_X} g(x)\ \mathbb{P}(X = x)
$$

# Continuous Case

If $X$ is an [[Absolutely Continuous Random Variable|absolutely continuous random variable]], then:

$$
\mathbb{E}[Y] = \mathbb{E}[g(x)] = \int_\mathbb{R} g(x)\ f_X(x)\ dx
$$
