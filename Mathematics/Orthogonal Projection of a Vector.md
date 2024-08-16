---
date: 2022-05-16
type: 🧠
tags:
  - MAC/2/ÁL
---

**Topics:** [[Algebra]] - [[Orthonormal and Orthogonal Set]] - [[Vector]]

---

_**(definition)**_

Let $H \leq \mathbb{R}^n$ with an [[Orthonormal and Orthogonal Set|orthonormal]] [[basis]] $\{ u_1, \dots, u_k \}$.

If $v \in \mathbb{R}^n$, then the _orthogonal projection_ of $v$ on $H$, denoted as $\text{proj}_H v$, is defined as:

$$
\text{proj}_H v := \langle v, u_1 \rangle u_1 + \langle v, u_2 \rangle u_2 + \dots + \langle v, u_k \rangle u_k
$$

> [!note]- Note
> The orthogonal projection is [[Well-defined|well-defined]] and it does not depend on the basis choice.

# Projections and Orthonormal Bases

_**(theorem)**_

Let $\beta = \{ u_1, \dots, u_n \}$ be an orthonormal basis for $\mathbb{R}^n$. , and let $v \in R$. Then:

$$
v = \langle v, u_1 \rangle u_1 + \dots + \langle v, u_n \rangle u_n
$$

_**(theorem)**_

Let $H \leq \mathbb{R}^n$ have two orthonormal bases $\{ u_1, \dots, u_k \}$ and $\{ w_1, \dots, w_k \}$.

If $v \in \mathbb{R}^n$, then:

$$
\langle v, u_1 \rangle u_1 + \dots + \langle v, u_k \rangle u_k = \langle v, w_1 \rangle w_1 + \dots + \langle v, w_k \rangle w_k
$$
