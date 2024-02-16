---
date: 2022-08-18
type: 🧠
tags:
  - MAC/S3/MD
  - MAC/S4/TG
---

**Topics:** [[Discrete Mathematics]] - [[Relation]] - [[Graph]]

---

_**(definition)**_

A _digraph_ is a [[Graph|graph]] where all of its [[Edge|edges]] are directed (i.e. they are all [[Arc|arcs]]).

There are [[Types of Digraphs|several types of digraphs]] (🗺).

# Digraphs and Relations

We can graphically represent a given a [[Relation|relation]] $R$ in $A$ with a _digraph_.

A digraph is made out of the following elements:

- **Vertices:** each vertex is an element of $A$
- **Arcs**: if $(x,y) \in R$, an arc is drawn from the vertex of $x$ to the vertex of $y$
	- If $(x,x) \in R$, then we draw a curved arc from $x$ to itself; we call this a [[Loop|loop]].

We can use digraphs to [[Properties of Relations in their Representations|easily determine the properties of the relation]].

> [!example]-
>
> For instance, let $A = \{1, 2, 3, 4\}$ and $R$ be defined by $(x,y) \in R$ if $x \leq y$, $\forall\ x, y \in A$.
>
> Represented as a set, this relation is:
>
> $$
> R = \{ (1,1), (1,2), (1,3), (1,4), (2,2), (2,3), (2,4), (3,3), (3,4), (4,4) \}
> $$
>
> …and has the digraph:
>
> ![[Digraph-1.png|200]]
