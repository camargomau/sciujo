---
date: 2022-09-20
type: 🧠
tags:
  - MAC/3/MN1
---

**Topics:** [[Numerical Analysis]] - [[Numerical Method]]

---

The _secant method_ is an open [[Numerical Method|numerical method]] of linear interpolation that can solve equations. It's similar to the [[Newton Method|Newton method]].

# Procedure

It supposes that $f(x)$ is linear, and draws a [[Secant Line|secant line]] that passes through $f(x_{0})$ and $f(x_{1})$. However, unlike the Newton method and other methods (like the [[Bisection Method|bisection method]]), the interval $x_{0}$ and $x_{1}$ must not necessarily contain a root.

![[Secant Method-1.png]]

With the help of this image, we can visualise that:

$$
\frac{x_{1}- x_{2}}{f(x_{1})} = \frac{x_{1} - x_{0}}{f(x_{1})-f(x_{0})}
$$

…and from there:

$$
x_{2} = x_{1} - f(x_{1}) \frac{x_{1} - x_{0}}{f(x_{1})-f(x_{0})}
$$

Finally, in general, we have that:

$$
x_{k+1} = x_{k} - f(x_{k}) \frac{x_{k-1} - x_{k}}{f(x_{k-1})-f(x_{k})}
$$

> [!tip]- Linearity of $f(x)$
> Notice that, if the function was linear, the secant line would intersect the $x$ axis exactly on the root.
>
> However, since $f(x)$ is rarely linear, the intersection of the secant line will not be the root, _but_ it will be close.
