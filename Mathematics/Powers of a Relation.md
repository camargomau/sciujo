---
date: 2022-08-30
type: 🧠
tags:
  - MAC/S3/MN1
---

**Topics:** [[Discrete Mathematics]] - [[Relation]]

---

_**(definition)**_

Let $R$ be a [[Relation|relation]] on a [[Set|set]] $A$. We define:

$$
R^{1} = R
$$

$$
R^{n} = R \circ R^{n-1}
$$

…where $\circ$ denotes [[Composition of Relations|relation composition]].

> [!example]-
>
> Let $A = \{1, 2, 3, 4\}$ and $R = \{(1,2), (1,3), (2,4), (3,2)\}$.
>
> We have that:
>
> - $R \circ R = \{(1,4), (1,2), (3,4)\}$
> - $R^{3} = R \circ R^{2} = \{(1,4)\}$
>
> …and that:
>
> - $R^{n} = \varnothing$ for $n \geq 4$
