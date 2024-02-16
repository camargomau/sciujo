---
date: 2023-02-17
type: 🧠
tags:
  - MAC/S4/C4
---

**Topics:** [[Arc Length]] - [[Vector-Valued Function]]

---

_**(definition)**_

Let $\sigma$ be the [[Curve|curve]] traced out by the following [[Vector-Valued Function|vector-valued function]] in the [[Interval|interval]] $a \leq t \leq b$:

$$
r(t) = \langle x_{1}(t), x_{2}(t), \dots, x_{n}(t) \rangle
$$

We define the _arc length parameter_, denoted $s$, to be the arc length of the portion of the curve that goes from $u = a$ to $u = b$. That is:

$$
s(t) := \int_a^t \sqrt{[x_1'(u)]^2 + [x_2'(u)]^2 + \dots + [x_n'(u)]^2} \ du
$$

…or, more simply, with [[Derivative of a Vector-Valued Function|its derivative]] and [[Norm|norm]], the arc length parameter $s$ is given by:

$$
s(t) = \int_a^t \| r'(u) \|\ du
$$

> [!example]-
> For example, let's find the arc length parametrisation of the circle of radius 4 centred at the origin. We can parametrise such a circle with the following function in the interval $0 \leq 0 \leq 2 \pi$:
>
> $$
> r(t) = \langle r_1(t), r_2(t) \rangle = \langle 4 \cos(t), 4 \sin(t) \rangle
> $$
>
> For such a function, the arc length parameter $s$ is given by:
>
> $$
> \begin{align*}
> s(t) &= \int_0^t \sqrt{[r'(u)]^2 + [g'(u)]^2}\ du \\ &= \int_0^t \sqrt{-4\sin(u)]^2 + [4\cos(u)]^2}\ du \\ &= 4 \int_0^t 1\ du \\ &= 4t
> \end{align*}
> $$
>
> Notice that we are just calculating the arc length from $u = 0$ to $u = t$. In this case, we found that $s = 4t$, so $t = s/4$.
>
> Then, this same function, now with the arc length parameter, becomes:
>
> $$
> r(s) = \left\langle r_1\left(\frac{s}{4}\right), r_2\left(\frac{s}{4}\right) \right\rangle = \left\langle 4 \cos\left(\frac{s}{4}\right), 4 \sin\left(\frac{s}{4}\right) \right\rangle
> $$
>
> Effectively drawing the same curve (the circle of radius 4 centred at the origin) now in the interval $0 \leq s \leq 8 \pi$.

> [!tip]- Arc Length Parameter Intuitively
> Intuitively, we can see the arc length parameter as the parameter that makes the function draw the curve at a constant speed that corresponds to its arc length. If this parameter draws a portion of a curve in exactly its arc length, then it's the arc length parameter.

_**(theorem)**_

We say that a given [[Parametrisation|parametrisation]] of a vector-valued function is an _arc length parametrisation_ if and only if its [[Derivative of a Vector-Valued Function|derivative]] is a [[Unit Vector|unit vector]].

That is, a parametrisation of a vector-valued function $r(t)$ is an arc length parametrisation if and only if $\| r'(t) \| = 1$.
