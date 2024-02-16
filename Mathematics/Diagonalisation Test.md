---
date: 2022-05-02
type: 🧠
tags:
  - MAC/S2/ÁL
---

**Topics:** [[Algebra]] - [[Diagonalisation of a Linear Transformation]] - [[Linear Transformation]] - [[Vector Space]]

---

Let $T : V \to V$ with $\dim(V) = n$.

$T$ is [[Diagonalisation of a Linear Transformation|diagonalisable]] if:

1. $f(t) = (-1)^n (t - \lambda_1) \dots (t - \lambda_n)$
2. The multiplicity of $\lambda$ is equal to $n - \text{ran}(T - \lambda I)$ for each eigenvalue

> [!example]-
>
> Let's see if $A = \begin{pmatrix} 3 & 1 & 0 \\ 0 & 3 & 0 \\ 0 & 0 & 4 \end{pmatrix}$. is diagonalisable.
>
> ## First condition
>
> We calculate the [[Characteristic Polynomial|characteristic polynomial]]:
>
> $$
> \det(A - \lambda I) = \det \begin{pmatrix} 3-\lambda & 1 & 0 \\ 0 & 3-\lambda & 0 \\ 0 & 0 & 4-\lambda \end{pmatrix}
> $$
>
> $$
> = (3-\lambda)^2 (4-\lambda)
> $$
>
> $$
> = (-1)(\lambda-3)^3 (\lambda-4)
> $$
>
> With that, we get that $\lambda_1 = 4$ (with a multiplicity of 1) and that $\lambda_2 = 3$ (with a multiplicity of 2).
>
> Since we get that $f(t) = (-1) (\lambda-3) (\lambda-3) (\lambda-4)$, then the first condition is satisfied.
>
> ## Second condition
>
> As for the second condition, we have to check for every [[Eigenvalues and Eigenvectors|eigenvalue]].
>
> ### First eigenvalue
>
> First, we have that $\lambda_1$ has a multiplicity of 1. Let's calculate $\text{ran} (A - \lambda_1 I)$:
>
> $$
> \text{ran} (A - \lambda_1 I) = \text{ran} \begin{pmatrix} -1 & 1 & 0 \\ 0 & -1 & 0 \\ 0 & 0 & 0 \end{pmatrix} = 2
> $$
>
> To find the range of a matrix, we counted the amount of columns that are [[linearly independent]].
>
> With that, we do get that $\dim(\mathbb{R}^3) - \text{ran} (A - \lambda_1 I) = 3 - 2 = 1 =$ the multiplicity of $l_1$. The second condition is satisfied with the first eigenvalue.
>
> ### Second eigenvalue
>
> We do the same we did for the first eigenvalue:
>
> $\text{ran} (A - \lambda_2 I) = \text{ran} \begin{pmatrix} 0 & 1 & 0 \\ 0 & 0 & 0 \\ 0 & 0 & 1 \end{pmatrix}$
>
> This time, we get that $\dim(\mathbb{R}^3) - \text{ran} (A - \lambda_2 I) = 3 - 2 = 1 \neq$ the multiplicity of $l_1$. The second condition is _not_ satisfied with the second eigenvalue.
>
> Since the second condition is not satisfied in this case, then it follows that $A$ isn't diagonalisable.
