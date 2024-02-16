---
date: 2022-04-18
type: 🧠
tags:
  - MAC/S2/ÁL
---

**Topics:** [[Algebra]] - [[Linear Transformation]]

---

_**(definition)**_

Let $T : V \rightarrow V$. We define the _determinant of the linear operator $T$_:

$$
\det(T) := \det([T]_\beta)
$$

…where the [[Associated Matrix of a Linear Transformation#Determinant of Associated Matrices|basis choice is irrelevant]].

> [!example]-
>
> Let $T : P_2(\mathbb{R}) \rightarrow P_2(\mathbb{R})$ be defined by $T(f) = f'$.
>
> How can we calculate $\det(T)$?
>
> We'll find $[T]_\beta$ with $\beta = \{1, x, x^2 \}$.
>
> We calculate $T(\beta)$ then build the matrix with the [[Coordinate Vector|coordinate vectors]]:
>
> - $T(1) = 0 = 0(1) + 0x + 0x^2$
> - $T(x) = 1 = 1(1) + 0x + 0x^2$
> - $T(x^2) = 2x = 0(1) + 2x + 0x^2$
>
> Then:
>
> $$
> [T]_\beta = \begin{pmatrix} 0 & 1 & 0 \\ 0 & 0 & 2 \\ 0 & 0 & 0 \end{pmatrix}
> $$
>
> And from there, we can calculate its determinant $\det([T]_\beta) = 0$, so we finally have that $\det(T) = 0$.

# Properties of the Linear Operator Determinant

1. $T$ is invertible $\iff$ $\det(T) \neq 0$
2. If $T$ is invertible, then $\det(T^{-1}) = [det(T)]^{-1}$
3. $\det(TU) = \det(T) \det(U)$, where $U : V \rightarrow W$
4. If $\lambda$ is a scalar and $\beta$ a basis for $V$, then:
	- $\det(T - \lambda I_V) = \det(A - \lambda I)$
	- …where $A = [T]_\beta$
