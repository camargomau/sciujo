---
date: 2022-07-12
type: 🧠
tags:
  - MAC/2/ÁL
---

**Topics:** [[Algebra]] - [[Linear Transformation]] - [[Eigenvalues and Eigenvectors]]

---

_**(theorem)**_

Let $T : V \rightarrow V$ with $V$ a [[Vector Space|vector space]] on $\mathbb{K}$ with finite [[dimension]]. Then, $T$ is [[Diagonalisation of a Linear Transformation|diagonalisable]] if and only if there exists a [[basis]] $\beta= \{ x_1, \dots, x_n \}$ for $V$ and [[scalars]] $\lambda_1, \lambda_2, \dots, \lambda_n$ (not necessarily distinct) such that:

$$
T(x_j) = \lambda_j x_j
$$

…with $1 \leq j \leq n$.

Under these circumstances, $[T]_\beta$ is diagonal:

$[T]_\beta = \begin{pmatrix}
   a_{1} &  &  & \\
   & a_{2} &  & \\
   &  &  \ddots & \\
   &  &   & a_{3}
 \end{pmatrix}
$

The vectors in $\beta$ are the [[Eigenvalues and Eigenvectors|eigenvectors]] of $T$, while the lambdas are its [[Eigenvalues and Eigenvectors|eigenvalues]].
