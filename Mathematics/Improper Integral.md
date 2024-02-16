---
date: 2022-04-20
type: 🧠
tags:
  - MAC/S2/C2
---

**Topics:** [[Calculus]] - [[Integral]]

---

_**(definition)**_

Let $f : [a, \infty) \to \mathbb{R}$ an [[integrable function]] $\forall [a, t] \subseteq [a, \infty)$.

If $\lim_{t \to \infty} \int_a^t f$ exists, then we say that:

$$
\int_a^\infty f
$$

…is the _improper integral_ of $f$ in $[a, \infty)$ and that:

$$
\int_a^\infty f = \lim_{t \to \infty} \int_a^t f\ dt
$$

> [!example]-
>
> Let's calculate $\int_1^\infty xe^{-x} dx$.
>
> According to this definition, we have that:
>
> $$
> \int_1^\infty xe^{-x} dx = \lim_{t \to \infty} \int_1^t xe^{-x}dx
> $$
>
> With the [[Fundamental Theorem of Calculus]], we can write:
>
> $$
> \int_1^\infty xe^{-x} dx = \lim_{t \to \infty} \left[ \left. -(x+1)e^{-x} \right \rvert_1^t \right] = \lim_{t \to \infty} \left( -\frac{t+1}{e^t} + \frac{2}{e} \right)
> $$
> Then by evaluating the limit, we get the final result
>
> $$
> \int_1^\infty xe^{-x} dx = \frac{2}{e}
> $$

If such a limit doesn't exist, then we say that such an integral diverges (i.e. it doesn't converge).

> [!example]- Example of non-convergence
> An example of an improper integral that diverges is $\int_0^\infty x\ dx$:
>
> $$
> \int_0^\infty x\ dx = \left. \lim_{t \to \infty} \frac{x^2}{2} \right \rvert_0^t = \lim_{t \to \infty} \left( \frac{t^2}{2} - 0 \right) = \text{diverges}
> $$

Note that improper integrals don't have to necessarily involve [[Infinity|infinity]]. We can also have improper integrals when we calculate the [[Integral|integral]] of a function as it approaches a vertical [[Asymptote|asymptote]].

> [!example]- Example of an improper integral that doesn't involve $\infty$
> Let $f(x) = \frac{\sqrt{1+x}}{\sqrt{1-x}}$; $f(1)$ is indeterminate; $f$ has a vertical asymptote on $x = 1$.
>
> As such, $\int_0^1 \frac{\sqrt{1+x}}{\sqrt{1-x}}$ is an improper integral:
>
> $$\int_0^1 \frac{\sqrt{1+x}}{\sqrt{1-x}}
> = \lim_{t \to 1} \int_0^t \frac{\sqrt{1+x}}{\sqrt{1-x}}$$
>
> $$
> = \lim_{t \to 1} \left[ \frac{\sqrt{1-t^2}}{2} + \arcsin \frac{\sqrt{1-t}}{\sqrt 2} - \left( \frac{1}{2} + \arcsin \frac{1}{\sqrt 2} \right) \right]
> $$
>
> $$
> = -\frac{1}{2} - \frac{\pi}{6}
> $$
