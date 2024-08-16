---
date: 2023-03-14
type: 🧠
tags:
  - MAC/4/TG
---

**Topics:** [[Digraph]] - [[Graph Theory]]

---

_**(definition)**_

A _symmetric digraph_ is a [[Digraph|digraph]] where, for every _connected_ pair of [[Vertex|vertices]] $(v_i, v_j)$, there exists an [[Arc|arc]] that goes $v_i \to v_j$ and another one that goes $v_j \to v_i$ (i.e. a pair of [[Recurring Arcs|recurring]] arcs).

> [!info]- Complete vs. Symmetric
> A [[Complete Digraph|complete digraph]] is very similar to a symmetric digraph. The difference is that a complete digraph contains a pair of recurring arcs between _every_ pair of vertices, but a symmetric digraph only contains a pair of recurring arcs where a connection already exists.
>
> All complete digraphs are [[Symmetric Digraph|symmetric]], but not all symmetric digraphs are complete.
