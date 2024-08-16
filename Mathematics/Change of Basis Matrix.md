---
date: 2022-04-04
type: 🧠
tags:
  - MAC/2/ÁL
---

**Topics:** [[Algebra]] - [[Vector Space]] - [[Basis]]

---

Let $\beta$ and $\beta'$ be ordered basis of $V$ a [[Vector Space|vector space]] on $\mathbb{K}$ with finite [[dimension]].

Let $Q = [I_V]_\beta^{\beta'}$ (i.e. the [[Associated Matrix of a Linear Transformation|associated matrix]] to the [[Identity Transformation|identity transformation]] of $V$), then:

$$
Q[v]_\beta = [v]_{\beta'} \qquad \forall\ v \in V
$$

That is, by multiplying $Q$ by the [[Coordinate Vector|coordinate vector]] of $v \in V$ under $\beta$, we get the coordinate vector of $v$ under $\beta'$.

We call $Q$ the _change of basis matrix_ from $\beta$ to $\beta'$. Note that $Q$ is invertible and that $Q^{-1}$ is the change of basis matrix from $\beta'$ to $\beta$.

> [!example]-
>
> Let $V = \mathbb{R}^2$ and let:
> - $\beta = \{ (1, 1), (1, -1) \}$
> - $\beta' = \{ (2, 4), (3, 1) \}$
>
> From here, we can represent the two elements of $\beta'$ as a linear combination of the elements of $\beta$:
>
> $$
> (2, 4) = 3(1, 1) + (-1)(1, -1)
> $$
>
> $$
> (3,1) = 2(1, 1) + 1(1, -1)
> $$
>
> Then, we can build a matrix with these scalars:
>
> $$
> Q = \begin{pmatrix} 3 & 2 \\ -1 & 1 \end{pmatrix}
> $$
>
> This matrix can be seen as _the matrix that represents elements of $\beta'$ as elements of $\beta$_.
>
> Now, with the second proposition of this theorem, we have that:
>
> $$
> [(2, 4)]_\beta = Q[(2, 4)]_{\beta'}
> $$
>
> So we can now easily get the coordinate vector of $v$ relative to $\beta$:
>
> $$
> [(2, 4)]_\beta = \begin{pmatrix} 3 & 2 \\ -1 & 1 \end{pmatrix} \begin{pmatrix} 1 \\ 0 \end{pmatrix} = \begin{pmatrix} 3 \\ -1 \end{pmatrix}
> $$
