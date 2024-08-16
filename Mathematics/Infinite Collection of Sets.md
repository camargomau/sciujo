---
date: 2022-08-26
type: 🧠
tags:
  - MAC/3/C3
---

**Topics:** [[Calculus]] - [[Set]] - [[Topology]]

---

_**(definition)**_

Let $A_{1}, A_{2}, \dots, A_{n}, \dots$ be an infinite collection of [[Set|sets]]. We define:

$$
\cup_{i=1}^{\infty} A_{i} = \{ x \in X \mid x \in A_{k}, \text{ for some } k \}
$$

$$
\cap_{i=1}^{\infty} A_{i} = \{ x \in X \mid x \in A_{k}, \forall k \in \mathbb{N} \}
$$

> [!example]- Example 1
> Let:
>
> - $A_{1} = (-1, 1)$
> - $A_{2} = (-\frac{1}{2}, \frac{1}{2})$
> - $A_{3} = (-\frac{1}{3}, \frac{1}{3})$
> - $A_{4} = (-\frac{1}{4}, \frac{1}{4})$
> - $A_{5} = (-\frac{1}{5}, \frac{1}{5})$
> - $\vdots$
> - $A_{n} = (-\frac{1}{n}, \frac{1}{n})$
> - $\vdots$
>
> We get that:
>
> $$
> \cap_{i = 1}^{\infty} A_{i} = \{0\}
> $$
>
> $$
> \cup_{i = 1}^{\infty} A_{i} = (-1, 1)
> $$

> [!example]- Example 2
> Let:
> - $B_{1} = (0, 1)$
> - $B_{2} = (1, 2)$
> - $B_{3}  = (2, 3)$
> - $\vdots$
> - $B_{n} = (n-1, n)$
> - $\vdots$
>
> We get that:
>
> $$
> \cap_{i=1}^{\infty} B_{i} = \varnothing
> $$
>
> $$
> \cup_{i=1}^{\infty} B_{i} = (0, \infty) - \mathbb{N}
> $$

# Union of Open Sets is Open

_**(theorem)**_

Let $A_{1}, A_{2}, \dots, A_{i}, \dots \subseteq \mathbb{R}^{n}$ be an infinite collection of [[Open Set|open sets]]. Then, we have that $\cup_{i=1}^{\infty} A_i$ (their [[Union|union]]) is also an open set.

# Intersection of Closed Sets is Closed

_**(theorem)**_

Let $A_{1}, A_{2}, \dots, A_{i}, \dots \subseteq \mathbb{R}^n$ be an infinite collection of [[Closed Set|closed sets]]. Then, we have that $\cap_{i=1}^{\infty} A_{i}$ (their [[Intersection|intersection]]) is also a closed set.
