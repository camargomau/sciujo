---
date: 2023-03-22
type: 🧠
tags:
  - MAC/4/C4
---

**Topics:** [[Calculus]] - [[Integral]]

---

> [!info]- Naming
> In all my notes, _path integral_ refers to the integral of a **scalar** function over a curve, while _[[Line Integral|line integral]]_ refers to the integral of a **vector field** over a curve.
>
> Some authors call both _line integrals_ (of a scalar field and of a vector field, respectively).

_**(definition)**_

Let $f : \mathbb{R}^3 \to \mathbb{R}$ be a [[Function|function]] and let $c$ be a [[Curve|curve]] in $\mathbb{R}^3$. $f$ returns a value for every point of $c$.

We define the _path integral_ of $f$ over $c$ as:

$$
\int_c f\ ds := \int_I (f \circ r)(s)\ ds = \int_a^b (f \circ r)(s)\ ds
$$

…where $s$ is the [[Arc Length Parameter|arc length parametrisation]] of $c$.

> [!info]- Area of a Surface
> Path integrals have many applications. We can use them to calculate the average of $f$ over the curve, the centre of mass of an object, among others, but its use for calculating the area of a surface is especially useful for understanding them.
>
> Let's first go back to the concept of traditional [[Integral|integrals]]. They allow us to calculate the area under a curve generated by a specific function. The "base" of that surface was a straight line, the $X$-axis, while the "height" of the surface was given by the function.
>
> Path integrals aren't much different: they allow us to calculate the area of the surface between $c$ and $f$. $c$, the curve, is the "base" of the surface, which is now not necessarily a straight line, while $f$ gives us the height of every point in that curve.

Path integrals have [[Path Integral Applications|many applications]].

_**(theorem)**_

Let $f : \mathbb{R}^3 \to \mathbb{R}$ be a [[Function|function]] and let $c$ be a [[Curve|curve]] in $\mathbb{R}^3$:

$$
\int_c f\ ds = \int_a^b (f \circ r)(t) \|r'(t)\|\ dt
$$

…where $r : [a, b] \to \mathbb{R}^3$ is _any_ parametrisation of the curve $c$.
