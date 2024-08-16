---
date: 2022-10-21
type: 🧠
tags:
  - MAC/3/C3
---

**Topics:** [[Differentiable Vectorial Function]] - [[Matrix]]

---

_**(definition)**_

In the context of [[Partial Derivative|partial derivatives]], the _Jacobian matrix_ for a [[Function|function]] $f : \mathbb{R}^{n} \to \mathbb{R}^{m}$ is defined as:

$$
J(x_{1}, x_{2}, \dots, x_{n}) =
\begin{pmatrix}
\frac{\partial f_1}{\partial x_1} & \frac{\partial f_1}{\partial x_2} & \dots & \frac{\partial f_1}{\partial x_n} \\
\vdots & \vdots & \ddots & \vdots \\
\frac{\partial f_m}{\partial x_1} & \frac{\partial f_m}{\partial x_2} & \dots & \frac{\partial f_m}{\partial x_n} \\
\end{pmatrix}
$$

…where $f = (f_{1}, f_{2}, \dots, f_{n})$.

> [!example]-
> Let $f : \mathbb{R}^{2} \to \mathbb{R}^{2}$ be defined by $f(x,y) = (2x+3y, -\cos(xy))$.
>
> We got:
>
> $$
> f_{1} = \mathbb{R}^{2} \to \mathbb{R}, \quad f_{1}(x,y)= 2x+3y
> $$
>
> $$
> f_{2} = \mathbb{R}^{2} \to \mathbb{R}, \quad f_{2}(x,y)= -\cos(xy)
> $$
>
> So our Jacobian matrix is:
>
> $$
> J(x,y) = \begin{pmatrix} \frac{\partial f_{1}}{\partial x} & \frac{\partial f_{1}}{\partial y} \\ \frac{\partial f_{2}}{\partial x} &  \frac{\partial f_{2}}{\partial y} \end{pmatrix}
> $$
>
> $$
> J(x,y) = \begin{pmatrix} 2 & 3 \\ y \sin(xy) & x \sin(xy) \end{pmatrix}
> $$
