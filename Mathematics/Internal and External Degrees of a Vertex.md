---
date: 2023-03-07
type: 🧠
tags:
  - MAC/S4/TG
---

**Topics:** [[Vertex Degree]] - [[Graph Theory]]

---

_**(definition)**_

When we have a vertex $v_i$ connected to an [[Arc|arc]], we define:

- Its _internal_ degree, denoted $d^-(v_i)$, as the amount of arcs that point to said vertex.
- Its _external_ degree, denoted $d^+(v_i)$, as the amount of arcs that point away from said vertex.

# Sum Theorem

Given a [[Digraph|digraph]] with $n$ vertices, the sum of the internal degrees of all its vertices is equal to the sum of all the external degrees of all its vertices:

$$
\sum_{i=1}^n d^+ (v_i) = \sum_{i=1}^n d^- (v_i) = e
$$

Both of these sums is equal to the amount of [[Edge|edges]] of the digraph.
