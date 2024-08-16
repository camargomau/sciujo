---
date: 2022-05-20
type: 🧠
tags:
  - MAC/2/C2
---

**Topics:** [[Calculus]] - [[Taylor Series]]

---

_**(definition)**_

Let $f \in C_\infty [a, b]$ be function that's [[Differentiability|differentiable]] $n$ times $\forall n \in \mathbb{N}$.

We define the _Taylor series_ of $f$ around $c \in [a, b]$ as:

$$
\sum_{n=1}^\infty \frac{f^n (c) (x-c)^n}{n!}
$$

The Taylor series of $f$ equals $f$ in all of its domain.

Notice the Taylor series can be seen as a [[Taylor Polynomial|Taylor polynomial]] of infinite degree.

> [!example]-
> For instance, let $f(x) = e^x$. The Taylor series of $f$ around $0$ is rather easy to calculate, since the derivative of $e^x$ is always itself, and $e^0 = 1$.
>
> The Taylor series of this function is:
> $$
> e^x = \sum_{n=0}^\infty \frac{x^n}{n!} = 1 + x + \frac{x^2}{2} + \frac{x^3}{3!} + \frac{x^4}{4!} + \dots + \frac{x^k}{k!} + \dots
> $$
>
>
