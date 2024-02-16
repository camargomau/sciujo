---
date: 2022-08-23
type: 🧠
tags:
  - MAC/S3/MD
---

**Topics:** [[Discrete Mathematics]]

---

Let $R : A \to B$ be a [[Relation|relation]], with $A = \{a_{1}, \dots, a_{n}\}$ and $B=\{b_{1}, \dots, b_{m}\}$.

We define the _relation matrix_ $M_{R} \in \{0, 1\}^{n\times m}$ (a [[Boolean Matrix|boolean matrix]]) with:

$$
M_{R}= (a_{ij}) =
\begin{cases}
1, \text{ if } a_{i}\ R\ b_{j} \\
0, \text{if } a_{i}\ \centernot R\ b_{j}
\end{cases}
$$

We can use this matrix to [[Properties of Relations in their Representations|easily determine the properties of the relation]].

> [!example]-
>
> Let $R = \{(1,1), (1,2), (1,3), (1,4), (2,2), (2,3), (2,4), (3,3), (3,4), (4,4) \}$.
>
> The matrix for $R$ is:
>
> $$
> \begin{pmatrix} 1 & 1 & 1 & 1 \\ 0 & 1 & 1 & 1 \\ 0 & 0 & 1 & 1 \\ 0 & 0 & 0 & 1 \end{pmatrix}
> $$
>
> Notice that we can tell that $R$ is [[Properties of Relations|reflexive]] since its matrix has $1$s in its diagonal.
