---
date: 2022-04-04
type: 🧠
tags:
  - MAC/2/ÁL
---

**Topics:** [[Algebra]] - [[Linear Transformation]] - [[Vector Space]] - [[Associated Matrix of a Linear Transformation]] - [[Coordinate Vector]]

---

_(theorem)_

Let $V, W$ be [[Vector Space|vector spaces]] on $\mathbb{K}$, and $T : V \rightarrow W$ a [[Linear Transformation|linear transformation]].

Let:

- $v \in V$
- $\beta = \{v_1, \dots, v_n\}$ a [[basis]] for $V$
- $\gamma = \{w_1, \dots, w_n\}$ a basis for $W$

Then:

$$
[T]_{\beta}^{\gamma}\ [v]_{\beta} = [T(v)]_{\gamma}
$$

That is, the product of the [[Associated Matrix of a Linear Transformation|associated matrix]] of $T$ and the [[Coordinate Vector|coordinate vector]] of $v$ is equal to the coordinate vector of $T(v)$.

> [!example]-
>
> Let $T : \mathbb{R}^3 \rightarrow \mathbb{R}^2$ and…
>
> $$
> [T]_{\beta}^{\gamma} = \begin{pmatrix} 1 & -1 & 0 \\ 2 & 0 & 0 \\ 3 & 4 & 1 \end{pmatrix}
> $$
>
> …where $\beta = \gamma = \{ (1, 0, 0), (1, 1, 0), (1, 1, 1) \}$.
>
> Let's find $T(2, 0, -1)$.
>
> First, we find the coordinate vector (under $\beta$) of this element:
>
> $$
> [(2, 0, -1)]_{\beta} = \begin{pmatrix} 2 \\ 1 \\ -1 \end{pmatrix}
> $$
>
> Then, we multiply:
>
> $$
> [T]_{\beta}^{\gamma}\ [(2, 0, -1)]_{\beta} = \begin{pmatrix} 1 & -1 & 0 \\ 2 & 0 & 0 \\ 3 & 4 & 1 \end{pmatrix} \begin{pmatrix} 2 \\ 1 \\ -1 \end{pmatrix}
> $$
>
> $$
> = \begin{pmatrix} 1 \\ 4 \\ 9 \end{pmatrix} = [T(2, 0, -1)]_{\gamma}
> $$
>
> Finally, with that, we can write:
>
> $$
> T(2, 0, -1) = 1(1, 0, 0) + 4(1, 1, 0) + 9(1, 1, 1)
> $$
>
> $$
> = (14, 13, 9)
> $$
