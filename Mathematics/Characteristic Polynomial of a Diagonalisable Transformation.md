---
date: 2022-04-29
type: 🧠
tags:
  - MAC/S2/ÁL
---

**Topics:** [[Eigenvalues and Eigenvectors]] - [[Algebra]]

---

_**(theorem)**_

Let $T : V \to V$ be a [[Diagonalisation of a Linear Transformation|diagonalisable]] on a [[Vector Space|vector space]] $V$, and let $f(t)$ be the [[Characteristic Polynomial|characteristic polynomial]] of $T$.

Then, $f(t)$ is broken down into a product of $n$ factors, all with a degree of 1. That is, there exist scalars $\lambda_1, \dots, \lambda_2$ (not necessarily distinct) such that:

$$
f(t) = (-1)^n (t-\lambda_1) \dots (t-\lambda_2)
$$

_**(note)**_

If $f(t)$ has no distinct [[Eigenvalues and Eigenvectors|eigenvalues]], then $f(t)$ has multiple [[Polynomial Zero|zeroes]].

> [!example]-
>
> Let $A = \begin{pmatrix} 1 & 1 & 0 \\ 0 & 1 & 3 \\ 0 & 0 & 2 \end{pmatrix}$
>
> We have that:
>
> $$
> f(t) = \det(A - \lambda I)
> $$
>
> $$
> f(t) = \det \begin{pmatrix} 1 - \lambda & 1 & 0 \\ 0 & 1 - \lambda & 3 \\ 0 & 0 & 2 - \lambda \end{pmatrix}
> $$
>
> $$
> f(t) = (1-\lambda)(1-\lambda)(2-\lambda)
> $$
>
> $$
> f(t) = (-1)(\lambda-1)(\lambda-1)(\lambda-2)
> $$
>
> $$
> f(t) = (-1)(\lambda-1)^2(\lambda-2)
> $$
>
> With that, we get that the zeroes of the characteristic polynomial are:
>
> - $\lambda_1 = 1$ (with a multiplicity of 2)
> - $\lambda_2 = 2$ (with a multiplicity of 1)
