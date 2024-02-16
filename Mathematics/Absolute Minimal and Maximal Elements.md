---
date: 2022-09-01
type: 🧠
tags:
  - MAC/S3/MN1
---

**Topics:** [[Discrete Mathematics]] - [[Relation]]

---

_**(definition)**_

Let $(X, \preceq)$ be a [[Partially Ordered Set|poset]].

- An element $m \in X$ is an _absolute [[Minimal and Maximal|maximal element]]_ if $x \preceq m$ for all $x \in X$
- An element $s \in X$ is an _absolute [[Minimal and Maximal|minimal element]]_ if $s \preceq x$ for all $x \in X$

> [!example]- Examples
> With $(K, \subseteq)$ given:
>
> $$
> K = \{\{x\}, \{x,y\}, \{w,x,y,z\}, \{y,z\}\}
> $$
>
> …notice that:
>
>  - $\{x\}$ is a minimal element, but it's not an absolute minimal element since $\{x\} \nsubseteq \{y,z\}$
>  - $\{w,x,y,z\}$ is a maximal element and an absolute maximal element
