---
date: 2022-05-18
type: 🧠
tags:
  - MAC/S2/ÁL
---

**Topics:** [[Algebra]] - [[Vector Space]] - [[Linear Transformation]]

---

_**(definition)**_

Let $T : \mathbb{R}^n \to \mathbb{R}^n$ be a [[Linear Transformation|linear transformation]].

We say that $T$ is _orthogonal_ if:

$$
\langle x, y \rangle = \langle T(x), T(y) \rangle \qquad \forall x, y \in \mathbb{R}^n
$$

_**(theorem)**_

If $T : \mathbb{R}^n \to \mathbb{R}^n$ is linear, then $T$ is orthogonal if and only if ([[Norm|norm]]):

$$
\| T(x) \| = \| x \| \qquad \forall x \in \mathbb{R}^n
$$

> [!example]-
>
> Let $T : \mathbb{R}^3 \to \mathbb{R}^3$ be defined as $T(x, y, z) := (x, y z)$ (the [[Identity Transformation|identity transformation]]).
>
> Is $T$ orthogonal?
>
> For $(x, y, z) \in \mathbb{R}^3$, we have that:
>
> $$
> \langle (x, y, z), (x, y, z) \rangle = x^2 + y^2 + z^2
> $$
>
> $$
> \langle T(x, y, z), T(x, y, z) \rangle = x^2 + y^2 + z^2
> $$
>
> Voilà, that tells us that $T$ is orthogonal>
