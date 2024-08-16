---
date: 2023-03-10
type: 🧠
tags:
  - MAC/4/C4
---

**Topics:** [[Vector Field]] - [[Calculus]]

---

_**(definition)**_

The _divergence_ of a [[Vector Field|vector field]] $F(x,y,z) = \langle F_1(x,y,z), F_2(x,y,z), F_3(x,y,z) \rangle$ is the scalar [[Function|function]]:

$$
\text{div}\ F(x,y,z) = \frac{\partial F_1}{\partial x} + \frac{\partial F_2}{\partial y} + \frac{\partial F_3}{\partial z}
$$

…defined at all points at which all the indicated [[Partial Derivative|partial derivatives]] exist.

> [!tip] Alternative Notation
> More simply, with a bit of [[Notation Abuse|notation abuse]], we can say that the divergence of a vector field $F$ is:
>
> $$
> \text{div}\ F = \nabla \cdot F
> $$
>
> …where $\nabla = \left\langle \frac{\partial}{\partial x}, \frac{\partial}{\partial y}, \frac{\partial}{\partial z} \right\rangle$; see [[Inner Product|inner product]].

Divergence tells us _how much_ the [[Vector|vectors]] in the vector field "grow" or "shrink".

When the divergence of a vector field is $0$, we say that the vector field is _incompressible_.
