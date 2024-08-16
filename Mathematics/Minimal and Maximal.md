---
date: 2022-09-01
type: 🧠
tags:
  - MAC/3/MD
---

**Topics:** [[Discrete Mathematics]] - [[Partially Ordered Set]]

---

_**(definition)**_

Let $(A, \preceq)$ be a [[Partially Ordered Set|poset]].

- An element $m \in A$ is a _maximal element_ of $(A, \preceq)$ if there isn't any $x \in A$ such that $m \prec x$
- An element $s \in A$ is a _minimal element_ of $(A, \preceq)$ if there isn't any $x \in A$ such that $x \prec s$

> [!example]- Examples
> - $(\mathbb{R}, \leq)$ doesn't have any minimal or maximal elements.
> - $(\mathbb{R}_{+}, \leq)$ has $0$ as its minimal element (if $\mathbb{R}_{+} = [0, \infty)$)
> - $(\mathbb{N}, \leq)$ has $0$ as its minimal element
> - $(\mathcal{P}(X), \subseteq)$ has $\varnothing$ as its minimal and $X$ as its maximal
> - $(\mathcal{P}(X), \\ \varnothing)$ has $\{a\}, \{b\}, \{c\}$ as its minimals, and $X$ as its maximals

> [!warning]- Unique Maximal
>
> We have can only have a unique maximal element in [[Total Order Relation|totally ordered]] sets.

There can also be [[Absolute Minimal and Maximal Elements|absolute minimal and maximal elements]] in posets.
