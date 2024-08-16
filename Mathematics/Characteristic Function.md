---
date: 2023-04-19
type: 🧠
tags:
  - MAC/4/PB
---

**Topics:** [[Probability]]

---

_**(definition)**_

Let $X$ be a [[Random Variable|random variable]].

The _characteristic function_ of $X$, denoted $\varphi_{X} : \mathbb{R} \to \mathbb{C}$, is defined as:

$$
\varphi_{X}(t) = \mathbb{E}[ e^{ itX } ]
$$

…where $i = \sqrt{ -1 }$, of course.

Characteristic functions have [[Properties of a Characteristic Function|several properties]].

# Discrete Case

_**(theorem)**_

Knowing the form of the [[Expected Value|expected value]] for a [[Discrete Random Variable|random variable]]. the characteristic function of such a random variable is:

$$
\varphi_{X}(t) = \sum_{x \in R_{X}} e^{ itx } f_{X}(x)
$$

# Continuous Case

_**(theorem)**_

Similarly, for an [[Absolutely Continuous Random Variable|absolutely continuous random variable]]:

$$
\begin{align}
\varphi_{X}(t) &= \int_{\mathbb{R}} e^{ itx } f_{X}(x) \ dx \\
&= \int_{\mathbb{R}} e^{ itx } \ df_{X}(x)
\end{align}
$$

_**(theorem)**_

The characteristic function for $X$ is also given by:

$$
\varphi_X(t) = \int \cos(tx)\ f_X(x) \ dx + i \int \sin(tx)\ f_X(x) \ dx
$$

> [!question]- Where from?
> Remember that $e^x$ can be expressed as a [[Taylor Series|Taylor series]] as follows:
>
> $$
> e^x = \sum_{n=0}^\infty \frac{x^n}{n!} = 1 + x + \frac{x^2}{2} + \frac{x^3}{6} + \dots
> $$
>
> Setting $x = iy$, with $y \in \mathbb{R}$, we get:
>
> $$
> \begin{align*}
> e^{iy} &= 1 + (iy) + \frac{(iy)^2}{2!} + \dots \\
> &= \left( 1 - \frac{y^2}{2!} + \frac{y^4}{4!} - \dots \right) + i \left( y - \frac{y^3}{3!} + \frac{y^5}{5!} - \dots \right) \\
> &= \cos(y) + i\sin(y)
> \end{align*}
> $$
>
> The latter equivalence holding true due to the representation of $\cos(y)$ and $\sin(y)$ as Taylor series.
