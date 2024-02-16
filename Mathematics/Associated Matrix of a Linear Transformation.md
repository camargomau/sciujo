---
date: 2022-03-28
type: 🧠
tags:
  - MAC/S2/ÁL
aliases:
  - associated-matrix
---

**Topics:** [[Algebra]] - [[Linear Transformation]]

---

Given a [[Linear Transformation|linear transformation]] $T : V \rightarrow W$, the associated matrix of $T$ is a matrix that represents $T$ on the [[basis|bases]] of $V$ and $W$.

This matrix can be used to transform elements by [[Product of an Associated Matrix and a Coordinate Vector|having it multiply the respective coordinate vector]].

[[Associated Matrix of Operated Transformations|Operated]] and [[Associated Matrix of Composed Transformations|composed]] transformations can also have an associated matrix.

# Definition

Given:

- $V, W$ vector spaces with finite [[dimension]]
- $\beta = \{ x_1, \dots, x_n \}$ a basis of $V$
- $\gamma = \{y_1, \dots, y_n \}$ a basis of $W$
- A linear transformation $T : V \rightarrow W$

The associated matrix is a matrix $A \in M_{m \times n} (\mathbb{K})$ that contains elements $a_{ij} \in \mathbb{K}$ such that:

$$
T(x_j) = \sum_{i = 1}^n a_{ij} y_j,\ \ 1 \leq j \leq n
$$

Such a matrix is denoted by also $[A]_{\beta}^{\gamma}$, and is also known as a basis change matrix (_matriz de cambio de base_).

# Construction

To build the associated matrix of a linear transformation $T$, we can follow three steps:

1. Transform each one of the elements in $\beta$
2. Under $\gamma$, find the [[Coordinate Vector|coordinate vectors]] of the transformed elements
3. Build the matrix by using these coordinate vectors as its columns, in order.

> [!example]-
>
> Given the following linear transformation:
>
> $$
> T : P_3(\mathbb{R}) \rightarrow P_2(\mathbb{R})
> $$
>
> T(f(x)) := f'(x),\ f \in P_3(\mathbb{R})$$
>
>  …we have the bases of $V$ and $W$:
>
> - $\beta = \{ 1, x, x^2, x^3 \}$ for $P_3(\mathbb{R})$
> - $\gamma = \{ 1, x, x^2 \}$ for $P_2(\mathbb{R})$
>
> Let's find the associated matrix of $T$.
>
> We can further simplify the three steps by transforming each one of the elements in $\beta$, directly representing them as a [[linear combination]] of the elements in $\gamma$:
>
> - $T(1) = 0 = 0(1) + 0(x) + 0(x^2)$
> - $T(x) = 1 = 1(1) + 0(x) + 0(x^2)$
> - $T(x^2) = 2x = 0(1) + 2(x) + 0(x^2)$
> - $T(x^3) = 3x^2 = 0(1) + 0(x) + 3(x^2)$
>
> …and then taking the coefficients to build the associated matrix:
>
> $$
> [T]_{\beta}^{\gamma} = \begin{pmatrix} 0 & 1 & 0 & 0 \\ 0 & 0 & 2 & 0 \\ 0 & 0 & 0 & 3 \end{pmatrix}
> $$

# Determinant of Associated Matrices

_**(theorem)**_

Let $T : V \rightarrow V$. Let $\beta$ and $\beta'$ be [[basis|bases]] for $V$. of $T$ under different bases. We have that:

$$
\det([T]_\beta) = \det([T]_{\beta'})
$$
