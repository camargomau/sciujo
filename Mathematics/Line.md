---
date: 2022-03-29
type: 🧠
tags:
  - MAC/2/GE
aliases:
  - line
  - lines
---

**Topics:** [[Line]] - [[3D Space]]

---

Let $p = (x_1, x_2, x_3)$ be a [[point]] in $\mathbb{R}^3$ and $V = (v_1, v_2, v_3)$ a non-zero [[vector]] in $\mathbb{R}^3$.

# Vectorial Representation

In its vectorial representation, the line that goes through the point $P$ in the direction of the vector $V$ is the [[set]]:

$l = \{ P + tV \mid t \in \mathbb{R} \}$

This set can also be written as follows:

$$
l = \{ (x_1, x_2, x_3) + t(v_1, v_2, v_3) \mid t \in \mathbb{R} \}
$$

$$
l = \{ (x_1+tv_1, x_2+tv_2, x_3+tv_3) \mid t \in \mathbb{R} \}
$$

# Parametric Representation

In its parametric representation, the line that goes through the point $P$ in the direction of the vector $V$ is:

$$
l = \begin{cases}
x = x_1 + tv_1 \\
y = x_2 + tv_2 \\
z = x_3 + tv_3
\end{cases}
$$

# Symmetric Representation

In its symmetric representation, the line that goes through the point $P$ in the direction of the vector $V$ is:

$$
\frac{x-x_1}{v_1} = \frac{y-x_2}{v_2} = \frac{z-x_3}{v_3}
$$

> [!warning]- Beware!
>
> This representation only works if $v_1, v_2, v_3 \neq 0$.

> [!example]- If there is no $t$
> If you have a line that doesn't have $t$ in one of its arguments, then the symmetric representation changes.
>
> For example, the following line:
>
> $$
> l = \begin{cases} x = 2 \\ y = -9 - 9t \\ z = 3 - 3t \end{cases}
> $$
>
> …as the symmetric representation:
> $$
> \frac{y+9}{-9} = \frac{z-3}{-3}; x = 2
> $$
>
> And the line:
>
> $$
> l = \begin{cases} x = 5 \\ y = 9 - 9t \\ z = -10 \end{cases}
> $$
>
> …has the symmetric representation:
>
> $$
> t = \frac{y-9}{-9}; x = 5; z = -10
> $$

# Line Through the Origin

When $P = (0, 0, 0)$, then we call such a line a _line that goes through the [[origin]]_. This line in its vectorial representation is:

$$
l = \{ tV \mid t \in \mathbb{R} \}
$$

$$
l = \{ (tv_1, tv_2, tv_3 \mid t \in \mathbb{R}) \}
$$

# Line Through Two Points

The line that passes through two points $P = (x_1, x_2, x_3)$ and $R = (y_1, y_2, y_3)$ is, in its vectorial representation:

$$
l = \{ P + t(R-P) \mid t \in \mathbb{R} \}
$$
