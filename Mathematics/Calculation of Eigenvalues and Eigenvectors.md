---
date: 2022-04-20
type: 🧠
tags:
  - MAC/2/ÁL
---

**Topics:** [[Algebra]] - [[Linear Transformation]]

---

# Calculation of Eigenvalues

_**(theorem)**_

Let $T : V \rightarrow V$ with $V$ a vector space on $\mathbb{K}$ with finite [[dimension]].

A scalar $\lambda \in \mathbb{K}$ is an [[Eigenvalues and Eigenvectors|eigenvalue]] of $T$ if and only if $\det(T - \lambda I_V) = 0$ ([[Linear Operator Determinant]]).

_**(corollary)**_

Let $A \in M_{n \times n} (\mathbb{K})$ be the [[Associated Matrix of a Linear Transformation|associated matrix]] of $T$. A scalar $\lambda \in \mathbb{K}$ is an eigenvalue of $A$ (of $T$) if and only if $\det(A - \lambda I) = 0$.

## Examples

> [!example]- Example 1: Given the [[Associated Matrix of a Linear Transformation|associated matrix]]
> Let $A = \begin{pmatrix} 1 & 1 \\ 4 & 1 \end{pmatrix}$. Let's find the eigenvalues of $A$.
>
> First, we calculate $(A - \lambda I)$:
>
> $$
> \begin{pmatrix} 1 & 1 \\ 4 & 1 \end{pmatrix} - \lambda \begin{pmatrix} 1 & 0 \\ 0 & 1 \end{pmatrix} = \begin{pmatrix} 1-\lambda & 1 \\ 4 & 1-\lambda \end{pmatrix}
> $$
>
> Second, we calculate the [[determinant]] of this matrix:
>
> $\det(A - \lambda I) = \det \begin{pmatrix} 1-\lambda & 1 \\ 4 & 1-\lambda \end{pmatrix}$
> - $= (1 - \lambda)(1 - \lambda) - 4 = 1 - 2\lambda + \lambda^2 - 4$
> - $= \lambda^2 - 2\lambda - 3$
> - $= (\lambda - 3)(\lambda + 1)$
>
> Third, we make this last expression equal to $0$, to find the eigenvalues:
>
> $$
> (\lambda - 3)(\lambda + 1) = 0 \implies \lambda_1 = 3, \lambda_2 = -1
> $$
>
> Finally, with that we get that the eigenvalues are
> $\lambda_1 = 3$ and $\lambda_2 = -1$.

> [!example]- Example 2: Given the [[Linear Transformation|linear transformation]]
> Let $T : P_2(\mathbb{R}) \rightarrow P_2(\mathbb{R})$ be defined as follows:
>
> - $T(f(x)) = f(x) + xf'(x) + f'(x)$
>
> Let $\beta = \{ 1, x, x^2 \}$ be a basis for $P_2(\mathbb{R})$.
>
> Let's calculate the eigenvalues of $T$.
>
> #### First step
>
> We calculate $[T]_\beta$.
>
> - $T(1) = 1 + x(0) + 0x = 1 + 0x + 0x^2$
> - $T(x) = x + x(1) + 1 = 1 + 2x + 0x^2$
> - $T(x^2) = x^2 + x(2x) + 2x = 0 + 2x + 3x^2$
>
> With that:
>
> $$
> [T]_\beta = \begin{pmatrix} 1 & 1 & 0 \\ 0 & 2 & 2 \\ 0 & 0 & 3 \end{pmatrix}
> $$
>
> #### Second step
>
> Let's calculate $\det(T - \lambda I_V) = \det([T]_\beta - \lambda I)$:
>
> $$
> \det \left(\begin{pmatrix} 1 & 1 & 0 \\ 0 & 2 & 2 \\ 0 & 0 & 3 \end{pmatrix} - \begin{pmatrix} \lambda & 0 & 0 \\ 0 & \lambda & 0 \\ 0 & 0 & \lambda \end{pmatrix} \right)
> $$
>
> $$
> = \det \left(\begin{pmatrix} 1-\lambda & 1 & 0 \\ 0 & 2-\lambda & 2 \\ 0 & 0 & 3-\lambda \end{pmatrix} \right)
> $$
>
> $$
> = (1 - \lambda)(2 - \lambda)(3 - \lambda)
> $$
>
> $$
> = -(\lambda - 1)(\lambda - 2)(\lambda - 3)
> $$
>
> #### Third step
>
> We make this last expression we got equal to 0:
> $$
> -(\lambda - 1)(\lambda - 2)(\lambda - 3) = 0 \implies \lambda_1 = 1, \lambda_2 = 2, \lambda_3 = 3
> $$
>
> Finally, with that we have that the eigenvalues are $\lambda_1 = 1$, $\lambda_2 = 2$ and $\lambda_3 = 3$.

# Calculation of Eigenvectors

_**(theorem)**_

Let $T : V \rightarrow V$ and let $\lambda$ be an eigenvalue of $T$.

A vector $x \in V$ is an [[Eigenvalues and Eigenvectors|eigenvector]] of $T$ (that corresponds to $\lambda)$ if and only if $x \neq 0$ and $x \in \ker(T - \lambda I)$.

> [!example]- Example 1
> Let $A = \begin{pmatrix} 1 & 1 \\ 4 & 1 \end{pmatrix}$
>
> We have that $\lambda_1 = 3$, $\lambda_2 = -1$ (we calculated these in [[Calculation of Eigenvalues and Eigenvectors#Examples|example 1 for the calculation of eigenvectors]]).
>
> ### Eigenvector corresponding to $\lambda_1 = 3$
>
> We'll calculate the eigenvector that corresponds to $\lambda_1 = 3$:
>
> $$
> B = A - \lambda_1 I = \begin{pmatrix} 1 & 1 \\ 4 & 1 \end{pmatrix} - 3 \begin{pmatrix} 1 & 0 \\ 0 & 1 \end{pmatrix}
> $$
>
> $$
> = \begin{pmatrix} 1 & 1 \\ 4 & 1 \end{pmatrix} - \begin{pmatrix} 3 & 0 \\ 0 & 3 \end{pmatrix}
> $$
>
> $$
> = \begin{pmatrix} -2 & 1 \\ 4 & -2 \end{pmatrix}
> $$
>
> Let $x = \begin{pmatrix} x_1 \\ x_2 \end{pmatrix} \in \mathbb{R}^2$ be an eigenvector that corresponds to $\lambda_1 = 3 \iff x \neq 0$ and $x \in \ker(L_B)$. That is:
>
> $$
> \begin{pmatrix} -2 & 1 \\ 4 & -2 \end{pmatrix} \begin{pmatrix} x_1 \\ x_2 \end{pmatrix} = \begin{pmatrix} 0 \\ 0 \end{pmatrix}
> $$
>
> $$
> \implies \begin{pmatrix} -2x_1 + x_2 \\ 4x_1 - 2x_2 \end{pmatrix} = \begin{pmatrix} 0 \\ 0 \end{pmatrix}
> $$
>
> From that, we have:
>
> - $-2x_1 + x_2 = 0 \implies x_2 = 2x_1$
> - $4x_1 - 2x_2 = 0 \implies 2x_2 = 4x_1 \implies x_2 = 2x_1$
>
> Therefore, the solutions to the system take the form $x_2 = 2x_1$. We can write that as:
>
> $$
> \begin{pmatrix} x_1 \\ 2x_1 \end{pmatrix} = x_1 \begin{pmatrix} 1 \\ 2 \end{pmatrix}
> $$
>
> And with that, we finally get that the eigenvector that corresponds to $\lambda_1$ is $\begin{pmatrix} 1 \\ 2 \end{pmatrix}$.
>
> ### Eigenvector corresponding to $\lambda_2 = -1$
>
> We'll calculate the vector that corresponds to $\lambda_2 = -1$.
>
> $$
> B = A - \lambda_2 I = \begin{pmatrix} 1 & 1 \\ 4 & 1 \end{pmatrix} - (-1) \begin{pmatrix} 1 & 0 \\ 0 & 1 \end{pmatrix}
> $$
>
> $$
> = \begin{pmatrix} 1 & 1 \\ 4 & 1 \end{pmatrix} - \begin{pmatrix} -1 & 0 \\ 0 & -1 \end{pmatrix}
> $$
>
> $$
> = \begin{pmatrix} 2 & 1 \\ 4 & 2 \end{pmatrix}
> $$
>
> Let $x = \begin{pmatrix} x_1 \\ x_2 \end{pmatrix} \in \mathbb{R}^2$ be an eigenvector that corresponds to $\lambda_2 = -1$, if and only if $x \neq 0$ and $x \in \ker(L_B)$. That is:
>
>  $$\begin{pmatrix} 2 & 1 \\ 4 & 2 \end{pmatrix} \begin{pmatrix} x_1 \\ x_2 \end{pmatrix} = \begin{pmatrix} 0 \\ 0 \end{pmatrix}$$
>
> $$
> \implies \begin{pmatrix} 2x_1 + x_2 \\ 4x_1 + 2x_2 \end{pmatrix} = \begin{pmatrix} 0 \\ 0 \end{pmatrix}
> $$
>
> From that, we have:
>
> - $2x_1 + x_2 = 0 \implies x_2 = -2x_1$
> - $4x_1 - 2x_2 = 0 \implies 2x_2 = -4x_1 \implies x_2 = -2x_1$
>
> Therefore, the solutions to the system take the form $x_2 = -2x_1$. We can write that as:
>
> $$
> \begin{pmatrix} x_1 \\ -2x_1 \end{pmatrix} = x_1 \begin{pmatrix} 1 \\ -2 \end{pmatrix}
> $$
>
> And with that, we finally get that the eigenvector that corresponds to $\lambda_2$ is $\begin{pmatrix} 1 \\ -2 \end{pmatrix}$.
>
> ### Conclusion
>
> The eigenvectors of the [[Linear Transformation|linear transformation]] whose associated matrix is $A$ are:
>
> - $\begin{pmatrix} 1 \\ -2 \end{pmatrix}$, corresponding to $\lambda_1 = 3$
> - $\begin{pmatrix} 1 \\ 2 \end{pmatrix}$, corresponding to $\lambda_2 = -1$

> [!tip]- Example 1 - Uses for these eigenvectors
> _(concerning example 1)_
>
> The set that contains only the found eigenvectors is a [[basis]] for $V$:
>
> $$
> \left\{ \begin{pmatrix} 1 \\ -2 \end{pmatrix}, \begin{pmatrix} 1 \\ 2 \end{pmatrix} \right\}
> $$
>
> We can build the $Q$ matrix such that $A = Q^{-1}\ B\ Q$ (with $B$ a diagonal matrix; [[Diagonalisation of a Linear Transformation|diagonalisation]]) by using the eigenvectors as columns:
>
> $$
> Q = \begin{pmatrix} 1 & 1 \\ 2 & -2 \end{pmatrix}
> $$

# No Eigenvalues

There can be linear operators that, depending on the vector space field, can have eigenvalues or not.

> [!example]-
>
> Let $A = \begin{pmatrix} = 0 & -1 \\ 1 & -\lambda \end{pmatrix}$.
>
> Let's set $\det(A - \lambda I) = 0$ to find the eigenvalues:
>
> $$
> \det \begin{pmatrix} \lambda & -1 \\ 1 & -\lambda \end{pmatrix} = 0
> $$
>
> $$
> (-\lambda)(-\lambda) + 1 = 0
> $$
>
> $$
> \lambda^2 + 1 = 0
> $$
>
> Upon solving this quadratic equation, we get that $\lambda_{1, 2} = \pm i$. Note how these eigenvalues exist in $\mathbb{C}$, but not in $\mathbb{R}$.
