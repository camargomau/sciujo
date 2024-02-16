---
date: 2022-08-18
type: 🗺
---

[[Graph|Graphs]] can be of several types.

# Basic Graphs

- A graph with only [[Arc|arcs]] is called a _directed graph_, while a graph with no arcs is called a _non-directed graph_. A graph with both arcs and non-directed edges is called a _mixed graph_.

	- These two concepts help us define a [[Subjacent Graph|subjacent graph]].

- A _null graph_ is a graph that has no vertices or edges.

- A _trivial graph_ is a graph that consists of a single vertex with no edges.

- A _proper graph_ is a graph with an edge that joins two different vertices.

- A _general graph_ (or _pseudo-graph_) is a graph that consists of at least one loop or at least one [[Multi-Edge|multi-edge]].

- A _multi-graph_ (or _loop-less graph_) is a graph that has at least one multi-edge, but no loops.

# Elegant Graphs

- A [[Simple Graph|simple graph]] is a graph with no multi-edges or loops.

- A [[Regular Graph|regular graph]] whose vertices all have the same [[Vertex Degree|degree]].

- A [[Complete Graph|complete graph]] is a graph where every vertex pair is joined by an edge.

# Connected Graphs

- A [[Connected Graph|connected graph]] is a graph where we can reach any vertex from any other one.

	- A [[Strongly Connected Graph|strongly connected graph]] is a connected graph where we can also reach any given vertex from itself.

# Bipartite Graphs

- A [[Bipartite Graph|bipartite graph]] is a graph that can be "separated" into two interconnected graphs

	- A [[Complete Bipartite Graph|complete bipartite graph]] is a bipartite graph where all the vertices of each subgraph are connected between each other.

# Subgraphs

A [[Subgraph|subgraph]] is a graph contained within another graph.

- [[Edge-Disjoint Subgraphs|Edge-disjoint subgraphs]] are subgraphs that don't share any edges.

- [[Vertex-Disjoint Subgraphs|Vertex-disjoint subgraphs]] are subgraphs that don't share any vertices.

When we erase most of the edges in a subgraph while keeping only the necessary ones to join all the vertices, we get an [[Expanded Subgraph|expanded subgraph]].
