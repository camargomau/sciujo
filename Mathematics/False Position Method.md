---
date: 2022-09-06
type: 🧠
tags:
  - MAC/3/MN1
---

**Topics:** [[Numerical Analysis]]

---

The _false position method_ is a closed [[Numerical Method|numerical method]] that tries to find the [[Function Zero|zeroes]] of a given [[Function|function]]. This method is similar to the [[Bisection Method|bisection method]], with the only difference between them being the way we choose the middle point.

# Procedure

To use this method, we first suppose that a zero of the function is between any two initial points $x_0$ and $x_1$, chosen such that $f(x_0)$ and $f(x_1)$ are of opposite signs.

Next, we draw a line from $f(x_0)$ to $f(x_1)$, and we call $x_{2}$ its intersection with the $x$ axis. In the same way we do for the [[Bisection Method|bisection method]], we will use $x_{2}$ and its relation to $x_{0}$ and $x_{1}$ to continue finding an approximation to the zero of the function.

That is, for the iterations that follow, if $f(x_{2})$ and $f(x_{0})$ have opposite signs, then we'll set $x_{1} = x_{2}$; if not, then we'll set $x_{0} = x_{2}$.

> [!question]- How to find $x_2$
> Let's first visualise the procedure for this method:
>
> ![[False Position Method-1.png]]
>
> Notice that, with the help of the green and brown triangle in the above image, we can tell that:
>
> $$
> \frac{x_{2}-x_{0}}{f(x_{0})} = \frac{x_{1}-x_{0}}{f(x_{0})-f(x_{1})}
> $$
>
> …so by isolating $x_2$, we get:
>
> $$
> x_{2} = x_{1} - f(x_{1}) \frac{x_{0}-x_{1}}{f(x_{0})-f(x_{1})}
> $$

# Similarities with the Bisection Method

## Approximation and Stopping

Since this method works similarly to the [[Bisection Method|bisection method]], it also yields just an approximation to the real value, so we have to [[Bisection Method#Solution and Approximation|define a margin of tolerance before starting]].

In the same way, we can use the [[Bisection Method#When to Stop|same conditions we used for the bisection method]] for stopping this method.

## Advantages and Disadvantages

The false position method has almost the same advantages and disadvantages as the bisection method, except for the fact that:

- **Advantage:** This method converges faster
- **Disadvantage:** The final interval is not always useful as an error bound
