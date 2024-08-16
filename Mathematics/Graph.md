---
date: 2023-02-02
type: 🧠
tags:
  - MAC/4/TG
aliases:
  - graph
  - graphs
  - Graphs
---

**Topics:** [[Graph Theory]]

---

A _graph_ $G = \{ V, E \}$ is a mathematical structure that consists of two finite [[Set|sets]] $V$ and $E$.

- The elements of $V$ are called [[Vertex|vertices or nodes]].
- The elements of $E$ are called [[Edge|edges]].
- The set of vertices must be a non-empty set, but the set of lines can empty.

We can use graphs to represent the relationship between different elements. A [[Digraph|digraph]] is an example of a graph.

Graphs can be of [[Types of Graphs|several types]] (🗺).

> [!info] Order and Cardinality
> The _order_ of $G$ is the cardinality of $V$, while the _size_ of $G$ is the cardinality of $E$.

> [!example]-
> The following is a graph with vertices $A, B, C, D$ and edges $f, g, h, i$:
>
> ![[Graph-1.png|400]]

# Degree Sequence

We denote the minimum [[Vertex Degree|vertex degree]] in a graph with $\delta_{min}$ or $\delta$, and the maximum with $\delta_{max}$ or $\Delta$.

We can represent graphs with the [[Increasing and Decreasing Sequence|non-increasing sequence]] of its vertices' degrees. Do note that two graphs with the same sequence aren't necessarily [[Isomorphic Graphs|isomorphic]].
