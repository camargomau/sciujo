---
date: 2022-05-16
type: 🧠
tags:
  - MAC/S2/ÁL
---

**Topics:** [[Algebra]] - [[Orthonormal and Orthogonal Set]] - [[Vector]]

---

_**(definition)**_

Let $H \in \mathbb{R}^n$. We define the _orthogonal complement of_ $H$, denoted as $H^\perp$, as:

$$
H^\perp = \{ x \in \mathbb{R}^n \ | \ \langle x, h \rangle = 0 \quad \forall\ h \in H \}
$$

# Properties

_**(theorem)**_

If $H \leq \mathbb{R}^n$, then:

1. $H^\perp \leq \mathbb{R}^n$
2. $H \cap H^\perp = \{ 0 \}$
3. $\dim(H^\perp) = n - \dim(H)$

# Orthogonal Complement and Orthogonal Projection

_**(theorem)**_ (relative to [[Orthogonal Projection of a Vector|orthogonal projection]])

Let $H \leq \mathbb{R}^n$ and let $v \in \mathbb{R}^n$.

Then, there exists a pair of vectors $h$ and $p$ such that $h \in H$, $p \in H^\perp$ and $v = h + p$.

In particular, if $h = \text{proj}_H v$ and $p = \text{proj}_H v$, then:

$$
v = h + p = \text{proj}_H v + \text{proj}_{H^\perp} v
$$
