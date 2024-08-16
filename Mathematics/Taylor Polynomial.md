---
date: 2022-05-09
type: 🧠
tags:
  - MAC/2/C2
---

**Topics:** [[Calculus]] - [[Polynomial]] - [[Function]]

---

_**(definition)**_

Let $f : \mathbb{R} \to \mathbb{R}$ be a [[Function|function]], with $n$ [[Derivative|derivatives]].

We define the degree $n$ _Taylor polynomial_ around $a \in \mathbb{R}$ as:

$$
P_f (n, a) = \sum_{i=0}^n \frac{f^i (a)}{i!} (x-a)^i
$$
…where $f^i(a)$ denotes the $i$th derivative of $f$ evaluated at the point $a$. Note that the zeroth derivative $f$ is defined to be $f$ itself, while $0!$ is defined to be $1$.

> [!example]-
>
> Let $f(x) = e^x$. We'll build $P_f(1,0)$ first, then $P_f(4, 0)$.
>
> Calculating the derivatives of $f$ is trivial, since the derivative of $e^x$ is always itself:
>
> - $f(x) = e^x$
> - $f'(x) = e^x$
> - $f''(x) = e^x$
> - $f'''(x) = e^x$
> - etc.
>
> Evaluating the derivatives at $0$ is also trivial:
>
> - $f(0) = 1$
> - $f'(0) = 1$
> - $f''(0) = 1$
> - $f'''(0) = 1$
> - etc.
>
> With all of this, we can now easily build $P_f(1,0)$:
>
> $$
> P_f(1,0) = 1 + (x-0)1 = 1 + x
> $$
>
> …and $P_f(4,0)$:
>
> $$
> P_f(4,0) = 1 + 1(x-0) + \frac{1}{2!}(x-0)^2 + \frac{1}{3!}(x-0)^3 + \frac{1}{4!}(x-0)^4
> $$
>
> $$
> P_f(4,0) = 1 + x + \frac{x^2}{2} + \frac{x^3}{3!} + \frac{x^4}{4!}
> $$
