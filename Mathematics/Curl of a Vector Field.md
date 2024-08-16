---
date: 2023-03-10
type: 🧠
tags:
  - MAC/4/C4
---

**Topics:** [[Vector Field]] - [[Calculus]]

---

_**(definition)**_

The _curl_ of a [[Vector Field|vector field]] $F(x,y,z) = \langle F_1(x,y,z), F_2(x,y,z), F_3(x,y,z) \rangle$ is the vector field:

$$
\text{curl}\ F := \left( \frac{\partial F_3}{\partial y} - \frac{\partial F_2}{\partial z} \right) \textbf{i} + \left( \frac{\partial F_1}{\partial z} - \frac{\partial F_3}{\partial x} \right) \textbf{j} + \left( \frac{\partial F_2}{\partial x} - \frac{\partial F_1}{\partial y} \right) \textbf{k}
$$

> [!tip] Alternative Notation
> More simply, with a bit of [[Notation Abuse|notation abuse]], we can say that the curl of a vector field $F$ is:
>
> $$
> \text{curl}\ F = \nabla \times F
> $$
>
> …where $\nabla = \left\langle \frac{\partial}{\partial x}, \frac{\partial}{\partial y}, \frac{\partial}{\partial z} \right\rangle$; see [[Cross Product|cross product]].
>
> That is:
>
> $$\text{curl}\ F =
> \begin{vmatrix}
> \textbf{i} & \textbf{j} & \textbf{k}  \\
> \frac{\partial}{\partial x} & \frac{\partial}{\partial y} & \frac{\partial}{\partial z}  \\
> F_1 & F_2 & F_3
> \end{vmatrix}$$

Curl tells us the rate of rotation of the [[Vector|vectors]] in a vector field.

When the curl of a vector field is $\vec 0$, we say that the vector field is _irrotational_.
