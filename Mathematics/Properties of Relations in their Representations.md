---
date: 2022-08-23
type: 🧠
tags:
  - MAC/3/MD
---

**Topics:** [[Discrete Mathematics]]

---

Let $R$ be a [[Relation|relation]] and $A$ be [[Matrix of a Relation|its matrix]].

We can use $A$ or the relation's [[Digraph|digraph]] to easily determine the [[Properties of Relations|properties]] of $R$:

1. **Reflexive** if and only if $A$ has $1$s in its diagonal.
2. **Symmetric** if and only if all arrows in the digraph are bidirectional.
3. **Antisymmetric** if and only if between any two vertices there is, at least, one arrow.
4. **Transitive** if and only if the digraph holds the property that if there exist arrows from $x$ to $y$ and from $y$ to $z$, then there's one from $x$ to $z$.
