---
date: 2022-05-06
type: 🧠
tags:
  - MAC/S2/ÁL
  - MAC/S3/C3
---

**Topics:** [[Algebra]] - [[Vector Space]] - [[Calculus]]

---

_**(definition)**_

Let $V$ be a [[Vector Space|vector space]] on $\mathbb{K}$ and let $\langle \cdot, \cdot \rangle : V \times V \to \mathbb{K}$ be a function.

We say that $\langle \cdot, \cdot \rangle$ is an _inner product_ if:

1. $\langle x, x \rangle \geq 0$, $\quad \forall\ x \in V$
2. $\langle x, x \rangle = 0 \iff x = 0$
3. $\langle x + y, z \rangle = \langle x, z \rangle + \langle y, z \rangle$, $\quad \forall\ x, y, z \in V$
4. $\langle \lambda x, y \rangle = \lambda \langle x, y \rangle$, $\quad \lambda \in \mathbb{K},\ x, y \in V$
5. $\langle x, y \rangle = \overline{ \langle y, x \rangle }$ (the [[Conjugate|conjugate]])

A vector space $V$ where an inner product is defined is called a _vector space with inner product_, and is denoted by $(V, \langle \cdot, \cdot \rangle)$.

> [!example]- Example 1 (traditional $\mathbb{R}^n$)
> In $(\mathbb{R}^n, +, \cdot)$ we define the inner product of $u = (u_1, u_2, \dots, u_n)$ and $v = (v_1, v_2, \dots, v_n)$ as:
>
> $$
> \langle u, v \rangle = u_1 v_1 + u_2 v_2 + \dots + u_n v_n
> $$
>
> This operation satisfies the aforementioned properties of an inner product.

> [!example]- Example 2
> Let $V = \mathcal{C}([a, b]) = \{ f: [a, b] \to \mathbb{R} \mid f \text{ is continuous in } [a, b] \}$
>
> Then, we define:
>
> $$\langle f, g \rangle := \int_a^b f(t) g(t) dt$$!-

Inner product helps us define [[Orthonormal and Orthogonal Set|orthonormal and orthogonal sets]].
