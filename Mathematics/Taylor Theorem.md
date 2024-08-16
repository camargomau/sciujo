---
date: 2022-05-13
type: 🧠
tags:
  - MAC/2/C2
---

**Topics:** [[Calculus]] - [[Taylor Polynomial]]

---

Let $f : [a, x] \to \mathbb{R}$ be a [[Function]] $C_{n+1}$ (i.e. [[Continuous Function|continuous]] $n+1$ times; [[Differentiability|differentiable]] $n+1$ times).

We define _the remainder_ as:
$$
R_{n, a}(x) := f(x) - \left(f(a) + f'(a)(x-a) + \dots + \frac{f^n (a) (x-a)^n}{n!} \right)
$$
That is, the remainder is the function minus its degree $n$ [[Taylor Polynomial|Taylor polynomial]].

Furthermore, we can represent the remainder in the following forms:

1. **Lagrange form:** for some $t \in (a, x),$

$$
R_{n, a}(x) = \frac{f^{n+1}(t)}{n!} (x-t)^n (x-a)
$$

1. **Cauchy form:** for some $t \in (a, x)$,

$$
R_{n, a}(x) = \frac{f^{n+1}(t)}{(n+1)!} (x-a)^{n+1}
$$

1. **Integral form:**

$$
R_{n, a}(x) = \int_a^x \frac{f^{n+1}(t)}{n!} (x-t)^n\ dt
$$

> [!example]- Example with application
> We'll use a neat example to show not only how the remainder can be used, but also what it could be useful for.
>
> Let $f(x) = e^x$. Then, we have that the [[Taylor Polynomial]] of $f$ of degree $1$ around $a = 0$ is:
>
> $$
> P_f(1, 0) = 1 + x
> $$
>
> …which approximates $e^x$ to a certain degree around $0$, of course. We can calculate the difference between this polynomial and actual $f$ by using the remainder:
>
> $$
> R_f(1, 0) = e^x - P_f(1, 0)
> $$
>
> $$
> R_f(1, 0) = e^x - (1 + x)
> $$
>
> Then, we can isolate $e^x$:
>
> $$
> e^x = (1 + x) + R_f(1, 0)
> $$
>
> …rewrite the remainder in its integral form:
>
> $$
> e^x = (1 + x) + \int_0^x e^t (x-t)\ dt
> $$
>
> …and when setting $x = 1$, we can approximate the value of $e$:
>
> $$
> e^1 = 2 + \int_0^1 e^t (1-t)\ dt
> $$
