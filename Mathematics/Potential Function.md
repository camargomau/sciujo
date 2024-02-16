---
date: 2023-03-08
type: 🧠
tags:
  - MAC/S4/C4
---

**Topics:** [[Vector Field]]

---

_**(definition)**_

Given $F: \mathbb{R}^n \to V_n$ a [[Vector Field|vector field]], we say that $f : \mathbb{R}^n \to \mathbb{R}$ is a _potential function_ of $F$ if:

$$
\nabla f = F
$$

…where $\nabla f$ denotes the [[Gradient|gradient]] of $f$.

> [!example]-
> Let $F(x,y) = \langle x, y \rangle$.
>
> Is $f : \mathbb{R}^2 \to \mathbb{R}$, $f(x,y) = \frac{x^2}{2} + \frac{y^2}{2}$ a potential function of $F$?
>
> Let's obtain its gradient:
>
> $$
> \nabla f = \left\langle \frac{\partial f}{\partial x}, \frac{\partial f}{\partial y} \right\rangle = \langle x, y \rangle = F
> $$
>
> As we can see, $\nabla f = F$, so $f$ is effectively a potential function of $F$.
>

When a vector field has a potential function, we say that it is _conservative_.
