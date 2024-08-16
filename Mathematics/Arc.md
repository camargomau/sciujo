---
date: 2023-02-07
type: 🧠
tags:
  - MAC/4/TG
aliases:
  - arc
  - head
  - tail
  - multi-arc
---

**Topics:** [[Graph]] - [[Edge]]

---

_**(definition)**_

An _arc_ is a [[Edge|directed edge]] that joins two [[Vertex|vertices]] together.

Given an arc $e$, the _head_ (denoted $head(e)$) is the vertex the arrow points to, while the _tail_ (denoted $tail(e)$) is the vertex the arrow points away from.

# Types

- Given a pair of arcs, we may have [[Recurring Arcs|recurring]] or [[Parallel Arcs|parallel]] arcs.

- When we have two different arcs that connect a same pair of vertices, but in different directions, we say that they are _oppositely directed arcs_.

- A _multi-arc_ is a set of two or more arcs that have the same head or tail. The multiplicity of a multi-arc is the number of arcs involved.
