---
date: 2022-03-31
type: 🧠
tags:
  - MAC/S2/GE
aliases:
  - parallel
---

**Topics:** [[Geometry]] - [[Line]] - [[3D Space]]

---

Two [[Line|lines]] $l_1, l_2$ in $\mathbb{R}^3$:
$$
l_1 = \{ P + tv  \mid t \in \mathbb{R} \}
$$

$$
l_2 = \{Q + su  \mid s \in \mathbb{R} \}
$$
…are parallel if and only if $u$ and $v$ are parallel. That is, if and only if $u$ and $v$ are multiples of each other ($\exists\ \lambda \in \mathbb{R}$ such that $u = \lambda v$).

> [!example]- Example 1
> Let:
>
> $$
> l_1 = \{ t(1,1,1) \mid t \in \mathbb{R} \}
> $$
>
> $$
> l_2 = \{ (1,1,1) + t(1,1,1) \mid t \in \mathbb{R} \}
> $$
>
> $l_1$ and $l_2$ are parallel because the vectors in their definition are the same one:
> $$
> u = v
> $$

> [!example]- Example 2
> Let:
>
> $$
> l_1: \frac{x-3}{2} = \frac{y-3}{5} = \frac{z-7}{4}
> $$
>
> $$
> l_2: \frac{x-4}{8} = \frac{y+9}{20} = \frac{z+11}{16}
> $$
>
> For $l_1$, we got $u = (2, 5, 4)$, For $l_2$, we got $v = (8, 20, 16)$.
>
> Since $v = 4u$, both vectors are parallel and thus, $l_1$ and $l_2$ are also parallel.
