---
date: 2022-03-31
type: 🧠
tags:
  - MAC/2/GE
aliases:
  - intersecting line
  - intersecting lines
---

**Topics:** [[Geometry]] - [[Line]] - [[3D Space]]

---

Let $l_1$ and $l_2$ be two [[Line|lines]] in $\mathbb{R}^3$.

We say $l_1$ and $l_2$ intersect on a point if they are different lines if there exists a point $R \in \mathbb{R}^3$ such that:

$$
l_1 \cap l_2 = \{ R \}
$$

# Procedure

Given two lines in its general [[Line#Vectorial Representation|vectorial representation]]:

$$
l_1 = \{ (P_1, P_2, P_3) + t(u_1, u_2, u_3) \mid t \in \mathbb{R} \}
$$

$$
l_2 = \{ (Q_1, Q_2, Q_3) + s(v_1, v_2, v_3) \}
$$

We can find their intersection by making them equal. This is the equation from where we start:

$$
(P_1, P_2, P_3) + t(u_1, u_2, u_3) = (Q_1, Q_2, Q_3) + s(v_1, v_2, v_3)
$$

With that, we get the system with two variables $t$ and $s$:

$$
\begin{cases}
P_1 + tu_1 = Q_1 + sv_1 \\
P_2 + tu_2 = Q_2 + sv_2 \\
P_3 + tu_3 = Q_3 + sv_3
\end{cases}
\implies
\begin{cases}
tu_1 - sv_1 = -P_1 + Q_1 \\
tu_2 - sv_2 = -P_2 + Q_2 \\
tu_3 - sv_3 = -P_3 + Q_3
\end{cases}
$$

Solving this system gives us the intersection of the two lines. We can get three cases:

1. There is one and only one solution $\implies$ the lines intersect ([[Two Line Cases|case 3]])
2. There are no solutions $\implies$ the lines never intersect
	- The lines _could_ be [[Parallel Lines|parallel]] or not ([[Two Line Cases|case 2]] or [[Two Line Cases|case 4]])
3. There are infinite solutions $\implies$ the lines are actually the same line (i.e. they intersect everywhere; [[Two Line Cases|case 1]])

> [!example]- Example 1
> Let:
>
> $$
> l_1: \frac{x-3}{2} = \frac{y-4}{5} = \frac{z-7}{4}
> $$
>
> $$
> l_2: \frac{x-4}{8} = \frac{y+9}{20} = \frac{z+11}{16}
> $$
>
> With these two lines, we get the system:
>
> $$
> \begin{cases} 2t - 8s = 1 \\ 5t - 20s = -13 \\ 4t - 16s = -18 \end{cases}
> $$
>
> To solve this system, we can remove one of the equations, and then see if the [[determinant]] of the corresponding matrix is $0$.
>
> For instance, if we remove the second equation we get:
>
> $$
> \begin{cases} 2t - 8s = 1 \\ 4t - 16s = -18 \end{cases}
> $$
>
> $$
> \implies \begin{vmatrix} 2 & -8 \\ 4 & -16 \end{vmatrix} = -32 + 32 = 0
> $$
>
> Since the determinant is $0$, then we can't work with these two equations. We shall then choose another combination of two equations and try and see if the corresponding determinant is non-zero.
>
> However, for these two lines, we get that all three possible determinants are $0$. In that case, then it follows that the two lines don't intersect (i)

> [!example]- Example 2
> Let:
>
> $$
> l_1: \frac{x-3}{2} = \frac{y-4}{5} = \frac{z-7}{4}
> $$
>
> $$
> l_2: \frac{x-4}{8} = \frac{y+9}{22} = \frac{z+11}{16}
> $$
>
> Or, in their [[Line#Vectorial Representation|vectorial representation]]:
>
> $$
> l_1 = \{ (3, 4, 7) + t(2, 5, 4) \mid t \in \mathbb{R} \}
> $$
>
> $$
> l_2 = \{ (4, -9, -11) + s(8, 22, 16) \mid s \in \mathbb{R} \}
> $$
>
> With these two lines, we get the system:
>
> $$
> \begin{cases} 2t - 8s = 1 \\ 5t - 22s = -13 \\ 4t - 16s = -18 \end{cases}
> $$
>
> To solve this system, we can remove one of the equations, and then see if the determinant of the corresponding matrix is $0$.
>
> For instance, if we remove the first equation we get:
>
> $$
> \begin{cases} 5t - 22s = -13 \\ 4t - 16s = -18 \end{cases}
> $$
>
> $$
> \implies \begin{vmatrix} 5 & -22 \\ 4 & -16 \end{vmatrix} = -80 + 88 = 8 \neq 0
> $$
>
> Since the determinant is non-zero, we can work with this specific two-equation system.
>
> Upon solving it with whichever method we find most convenient, we can find the solutions to these two equations are:
>
> - $t = -\frac{47}{2}$
> - $s = -\frac{19}{4}$
>
> When plugging these values into the equation from where we started:
> $$
> (P_1, P_2, P_3) + t(u_1, u_2, u_3) = (Q_1, Q_2, Q_3) + s(v_1, v_2, v_3)
> $$
> …we should get the intersection point.
>
> However, notice these two solutions won't solve the other equation, the one we removed earlier. As such, the system has no solution, and thus, the lines never intersect.
