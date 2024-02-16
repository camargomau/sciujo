---
date: 2022-04-29
type: 🧠
tags:
  - MAC/S2/ÁL
---

**Topics:** [[Eigenvalues and Eigenvectors]] - [[Algebra]]

---

_**(definition)**_

Let $T : V \to V$ and let $\lambda$ be an [[Eigenvalues and Eigenvectors|eigenvalue]] of $T$. We define:

$$
E_\lambda = \{ x \in V \mid T(x) = \lambda x \}
$$

$$
E_\lambda = \ker(T - \lambda I_V)
$$

…and call this set the _eigenspace that corresponds to the $\lambda$ eigenvalue_.

_**(note)**_

$E_\lambda$ is a [[Vector Subspace|vector subspace]] that contains $0$ and the eigenvectors of $T$ that correspond to $\lambda$.

The number of linearly independent eigenvectors of $T$ is the dimension of $E_\lambda$.

_**(theorem)**_

Let $T$ be a linear operator on $V$ a [[Vector Space|vector space]] with finite [[dimension]].

If $\lambda$ is an [[Eigenvalues and Eigenvectors|eigenvalue]] of $T$ with $k$ multiplicity, then:

$$
1 \leq \dim(E_\lambda) \leq k
$$

> [!example]-
>
> Let $T : P_2(\mathbb{R}) \to P_2(\mathbb{R})$ be defined $T(f) = f'$.
>
> What's $\dim(E_\lambda)$? To find out, let's follow the next steps:
>
> ## First step
>
> We build the [[Associated Matrix of a Linear Transformation|associated matrix]] of $T$ under the $\beta$, the canonical [[Basis|basis]]:
>
> $$
> [T]_\beta = \begin{pmatrix} 0 & 1 & 0 \\ 0 & 0 & 2 \\ 0 & 0 & 0 \end{pmatrix}
> $$
>
> ## Second step
>
> We find the eigenvalues of this transformation:
>
> $$
> \det([T]_\beta - \lambda I) = \det \begin{pmatrix} -\lambda & 1 & 0 \\ 0 & -\lambda & 2 \\ 0 & 0 & -\lambda \end{pmatrix} = -\lambda^3
> $$
>
> $$
> \implies -\lambda^3 = 0
> $$
>
> With that, we get that the eigenvalue is $\lambda = 0$ with a multiplicity of 3.
>
> ## Third step
>
> We'll find the eigenvectors that correspond to $\lambda$:
>
> $$
> E_\lambda = \ker( [T]_\beta - \lambda I) = \ker(T)
> $$
>
> $$
> E_\lambda = B = \begin{pmatrix} 0 & 1 & 0 \\ 0 & 0 & 2 \\ 0 & 0 & 0 \end{pmatrix}
> $$
>
> We equal $Bx = 0$ for some $x \in \mathbb{R}^3$ (a [[Coordinate Vector|coordinate vector]] of some $v \in V$):
>
> $$
> Bx = \begin{pmatrix} 0 & 1 & 0 \\ 0 & 0 & 2 \\ 0 & 0 & 0 \end{pmatrix} \begin{pmatrix} x_1 \\ x_2 \\ x_3 \end{pmatrix} = \begin{pmatrix} 0 \\ 0 \\ 0 \end{pmatrix}
> $$
>
> We solve and we get that (solve it)
>
> ## Fourth step
>
> The eigenspace is the space that only contains the eigenvectors that correspond to $\lambda$:
> Find a basis for the eigenspace, then it's easy to find the dimension
