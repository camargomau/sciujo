---
date: 2023-02-08
type: 🧠
tags:
  - MAC/S4/C4
---

**Topics:** [[Vector-Valued Function]] - [[Calculus]]

---

_**(definition)**_

Let $r(t) : \mathbb{R} \to \mathbb{R}^n$ be a [[Vector-Valued Function|vector-valued function]].

The [[Derivative|derivative]] $r'(t)$ of $r(t)$ is defined by:

$$
r'(t) := \lim_{\Delta t \to 0} \frac{r(t + \Delta t) - r(t)}{\Delta t}
$$

…for any values of $t$ for which the limit exists. When the limit as $t \to a$ exists, we say that $r$ is _differentiable_ at $t = a$.

[[Derivative of Operated Vector-Valued Functions|We can also derivate operated vector-valued functions]].

> [!warning]- Division
> The division in this definition is symbolic. As we can't divide vectors, It means the [[Scalar Multiplication|scalar multiplication]] of $r(t + \Delta t) - r(t)$ by $\frac{1}{\Delta t}$.

_**(theorem)**_

If we develop the limit given in this definition, we'll find that, if $r(t) = (r_1(t), r_2(t), \dots, r_n(t))$, then:

$$
r'(t) = \langle r_1'(t), r_2'(t), \dots, r_n'(t) \rangle
$$

# Graphical Representation

Graphically, the derivative of a vector-valued function is the _tangent vector_ to the function's curve at $t = a$.

![[Derivative of a Vector-Valued Function-1.png|300]]
