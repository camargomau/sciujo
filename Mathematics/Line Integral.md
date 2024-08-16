---
date: 2023-03-31
type: 🧠
tags:
  - MAC/4/C4
---

**Topics:** [[Calculus]] - [[Integral]]

---

> [!info]- Naming
> In all my notes, _[[Path Integral|path integral]]_ refers to the integral of a **scalar** function over a curve, while _line integral_ refers to the integral of a **vector field** over a curve.
>
> Some authors call both _line integrals_ (of a scalar field and of a vector field, respectively).

_**(definition)**_

Let $F$ be a [[Vector Field|vector field]] on $\mathbb{R}^3$ that is [[Continuous Function|continuous]] on the [[Curve|curve]] $c : [a, b] \to \mathbb{R}^3$.

We define the _line integral of $F$ along $c$_ as:

$$
\int_c F \cdot ds := \int_a^b (F \circ c)(t) \cdot c'(t) \ dt
$$
