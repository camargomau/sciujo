---
date: 2023-03-13
type: 🧠
tags:
  - MAC/S4/C4
---

**Topics:** [[Calculus]] - [[Vector-Valued Function]]

---

_**(definition)**_

Let $f : \mathbb{R}^3 \to \mathbb{R}$ be a [[Vector-Valued Function|vector-valued function]].

We define the _Laplacian_ of $f$ as:

$$
\nabla^2 f = \Delta f := \nabla \cdot (\nabla f)
$$

That is, the [[Divergence of a Vector Field|divergence]] of the function's [[Gradient|gradient vector]].

The Laplacian can be denoted by $\nabla^2$ or $\Delta$.

> [!tip] Alternative Notation
> Since $\nabla f = \left\langle \frac{\partial f}{\partial x},  \frac{\partial f}{\partial y}, \frac{\partial f}{\partial z} \right\rangle$, then:
>
> $$
> \begin{align*}
> \nabla \cdot (\nabla f) &= \left\langle \frac{\partial}{\partial x},  \frac{\partial}{\partial y}, \frac{\partial}{\partial z} \right\rangle \cdot \left\langle \frac{\partial f}{\partial x},  \frac{\partial f}{\partial y}, \frac{\partial f}{\partial z} \right\rangle \\[6pt]
> &= \frac{\partial^2 f}{\partial x^2} + \frac{\partial^2 f}{\partial y^2} + \frac{\partial^2 f}{\partial z^2}
> \end{align*}
> $$
