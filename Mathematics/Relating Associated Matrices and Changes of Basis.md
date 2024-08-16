---
date: 2022-04-04
type: 🧠
tags:
  - MAC/2/ÁL
---

**Topics:** [[Algebra]] - [[Linear Transformation]] - [[Vector Space]] - [[Associated Matrix of a Linear Transformation]]

---

Let $T : V \rightarrow W$ be a [[Linear Transformation|linear transformation]].

_**(theorem)**_

Let $\beta$ and $\beta'$ be ordered [[basis|bases]] of $V$, and $\gamma$ and $\gamma'$ ordered bases of $W$.

With the [[Associated Matrix of a Linear Transformation|associated matrices]] of $T$ under these bases, we have that:

$$
[T]_{\beta'}^{\gamma'} = P^{-1}\ [T]_\beta^\gamma\ Q
$$

…where $Q$ is the [[Change of Basis Matrix|change of basis matrix]] from $\beta'$ to $\beta$, and $P$ the change of basis matrix that from $\gamma'$ to $\gamma$.

> [!example]-
>
> Let $T : \mathbb{R}^3 \rightarrow \mathbb{R}^2$ be defined as $T(x, y,z) = (2x + y, x + y - z)$.
>
> Let $\beta$ and $\gamma$ be the standard basis of $\mathbb{R}^3$ and $\mathbb{R}^2$, respectively.
>
> Let:
> - $\beta' = \{ (2, 0, 0), (0, -1, 0), (0, 0, -2) \}$ be a basis of $\mathbb{R}^3$
> - $\gamma' = \{ (1, 1), (1, -1) \}$ be a basis of $\mathbb{R}^2$
>
> ## First step
>
> **First**, let's calculate $[T]_{\beta}^{\gamma}$ and $[T]_{\beta'}^{\gamma'}$.
>
> For $[T]_{\beta}^{\gamma}$, let's represent the elements of $\beta$ as a linear combination of the elements of $\gamma$:
> - $T(1, 0, 0) = (2, 1) = 2(1, 0) + 1(0, 1)$
> - $T(0, 1, 0) = (1, 1) = 1(1, 0) + 1(0, 1)$
> - $T(0, 0, 1) = (0, -1) = 0(1, 0) + (-1)(0, 1)$
> - With that:
> 	- $[T]_{\beta}^{\gamma} = \begin{pmatrix} 2 & 1 & 0 \\\ 1 & 1 & -1 \end{pmatrix}$
>
> For $[T]_{\beta'}^{\gamma'}$, let's represent the elements of $\beta'$ as a linear combination of the elements of $\gamma'$:
> - $T(2, 0, 0) = (4, 2) = 3(1,1) + 1(1, -1)$
> - $T(0, -1, 0) = (-1, -1) = (-1)(1,1) + 0(1,-1)$
> - $T(0, 0, -2) = (0, 2) = 1(1,1) + (-1)(1,-1)$
> - With that:
> 	- $[T]_{\beta'}^{\gamma'} = \begin{pmatrix} 3 & -1 & 1 \\ 1 & 0 & -1 \end{pmatrix}$
>
> ## Second step
>
> Second, let's find $Q$.
>
> For that, let's see the elements of $\beta'$ as a linear combination of the elements of $\beta$:
>
> - $(2, 0, 0) = 2(1, 0, 0) + 0(0, 1, 0) + 0(0, 0, 1)$
> - $(0, -1, 0) = 0(1, 0, 0) + (-1)(0, 1, 0) + 0(0, 0, 1)$
> - $(0, 0, -2) = 0(1, 0, 0) + 0(0, 1, 0) + (-2)(0, 0, 1)$
> - With that:
> 	- $Q = \begin{pmatrix} 2 & 0 & 0 \\ 0 & -1 & 0 \\ 0 & 0 & -2 \end{pmatrix}$
>
> ## Third step
>
> Third, to find $P^{-1}$, let's find $P$ first. Again, we do that by representing the elements of $\gamma'$ as a linear combination of the elements of $\gamma$:
>
> - (1, 1) = 1(1, 0) + 1(0, 1)$
> - $(1, -1) = 1(1, 0) + (-1)(0, 1)$
> - With that:
> 	- $P = \begin{pmatrix} 1 & 1 \\ 1 & -1 \end{pmatrix}$
>
> Since $\det(P) = -2 \neq 0$, we can invert $P$. We get that:
>
> $P^{-1} = \begin{pmatrix} \frac{1}{2} & \frac{1}{2} \\ \frac{1}{2} & -\frac{1}{2} \end{pmatrix}$
>
> Then we could multiply all of this to see that, in effect:
>
> $$
> [T]_{\beta'}^{\gamma'} = P^{-1}[T]_\beta^\gamma Q
> $$

_**(corollary)**_

Let $T : V \rightarrow V$ be a linear transformation, with ordered bases $\beta$ and $\beta'$. Then:

$$
[T]_{\beta'} = Q^{-1}[T]_\beta\ Q
$$

…where $Q$ is the basis change matrix from $\beta'$ to $\beta$.
