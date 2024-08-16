---
date: 2022-04-18
type: 🧠
tags:
  - MAC/2/ÁL
aliases:
  - Eigenvalue
  - eigenvalue
  - Eigenvalues
  - eigenvalues
  - Eigenvector
  - eigenvector
  - Eigenvectors
  - eigenvectors
---

**Topics:** [[Algebra]] - [[Linear Transformation]]

---

_**(definition)**_

Let $T : V \rightarrow V$ with $V$ a [[Vector Space|vector space]] on $\mathbb{K}$.

A non-null $x \in V$ is called an _eigenvector_ (_vector propio_) of $T$ if there exists a [[scalar]] $\lambda$ such that:

$$
T(x) = \lambda x
$$

We call $\lambda$ the _eigenvalue_ (_valor propio_) that corresponds to the eigenvector $x$.

Eigenvectors and eigenvalues [[Calculation of Eigenvalues and Eigenvectors|can be calculated by means of other theorems]].

# The Set of Eigenvectors is Linearly Independent

_**(theorem)**_

Let $T : V \to V$ and let $\lambda_1, \dots, \lambda_k$ be distinct eigenvalues of $T$.

If $x_1, \dots, x_k$ are eigenvectors of $T$ such that $x_j$ is the eigenvector that corresponds to $\lambda_j$ (given $1 \leq j \leq k$), then:

$$
\{ x_1, \dots, x_j \}
$$

…is a linearly independent set.

_**(corollary)**_

If $T : V \to V$ has $n$ distinct eigenvalues (with $\dim(V) = n)$, then $T$ is [[Diagonalisation of a Linear Transformation|diagonalisable]].

> [!tip]- Quick way to calculate $\det(A - \lambda)$
> Let's remember that, if $A$ is a _superior triangular matrix_:
>
> $$
> A = \begin{pmatrix} a_{11} & a_{12} & \dots & a_{1n} \\ 0 & a_{22} & \dots & a_{2n} \\ \vdots & \vdots & \ddots & \vdots \\ 0 & 0 & 0 & a_{nn} \end{pmatrix}
> $$
>
> Then:
>
> $$
> \det(A - \lambda I) = \det \begin{pmatrix} a_{11} - \lambda & a_{12} & \dots & a_{1n} \\ 0 & a_{22} - \lambda & \dots & a_{2n} \\ \vdots & \vdots & \ddots & \vdots \\ 0 & 0 & 0 & a_{nn} - \lambda \end{pmatrix}
> $$
>
> $$
> \det(A - \lambda I) = (a_{11} - \lambda)(a_{22} - \lambda)(a_{nn} - \lambda)
> $$

# Set of Eigenvectors as a Basis

The set that contains only the eigenvectors of a [[Linear Transformation]] $T : V \rightarrow V$ is a [[basis]] for $V$. When using this basis to build the [[Associated Matrix of a Linear Transformation|associated matrix]] of $T$, the [[Diagonal Associated Matrix|resulting matrix is diagonal]].

# Eigenvectors and Diagonalisation

Concerning the [[Diagonalisation of a Linear Transformation|diagonalisation of a linear transformation]], we can build the $Q$ matrix that diagonalises $A$ (the [[Associated Matrix of a Linear Transformation|associated matrix]] of the [[Linear Transformation|linear transformation]]) by using the eigenvectors as its columns.

**A condition necessary for diagonalisation is the existence of eigenvalues.**

For an example, refer to [[Calculation of Eigenvalues and Eigenvectors#Calculation of Eigenvectors|the uses of the eigenvalues of this example]].
