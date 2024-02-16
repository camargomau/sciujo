---
date: 2023-02-28
type: 🧠
tags:
  - MAC/S4/TG
---

**Topics:** [[Graph Theory]] - [[Graph]]

---

_**(definition)**_

A [[Graph|graph]] $g$ is a _subgraph_ of another graph $G$ when:

- All of the [[Vertex|vertices]] of $g$ are contained in $G$.
- Every [[Edge|edge]] in $g$ has the same terminal vertices in $G$.

> [!warning]- Exact Same Vertices and Edge Connections
> Beware! For a graph to be a subgraph of another one, it _must_ have the exact same vertices and edge connections, letter representation and all.

Subgraphs can be [[Edge-Disjoint Subgraphs|edge-disjoint]] or [[Vertex-Disjoint Subgraphs|vertex-disjoint]].

# Theorems

_**(theorem)**_

- A graph is a subgraph of itself
- A subgraph of a subgraph of $G$ is also a subgraph of $G$ ([[Properties of Relations|transitivity]])
- A single vertex of $G$ is a subgraph
- An edge with its terminal vertices (in $G$) is a subgraph of $G$

[[Edge-Disjoint Subgraphs]]
