---
type: 🏫
tags:
  - MAC/S4/TG
---

# Graphs

A [[Graph|graph]] is a structure that has a set of [[Vertex|vertices]] and a set of [[Edge|edges]]. Edges link together vertices. Graphs can be represented graphically:

![[Graph-1.png|300]]

There are [[Types of Graphs|several types of graphs]] (🗺), among them:

- The most important one is the [[Simple Graph|simple graph]].
- A simple graph whose vertices have all the same degree is called a [[Regular Graph|regular graph]].
- A graph where every vertex can be reached from any other one is a [[Connected Graph|connected graph]].

Just like many other mathematical structures, [[Isomorphic Graphs|graphs can be isomorphic]].

Graphs contained within other graphs are called [[Subgraph|subgraphs]].

- We can have [[Edge-Disjoint Subgraphs|edge-disjoint]] and [[Vertex-Disjoint Subgraphs|vertex-disjoint]] subgraphs.
- We can also have [[Expanded Subgraph|expanded subgraphs]].
- A [[Proper Subgraph|proper subgraph]] is a subgraph whose set of edges or vertices is a _proper_ subset of the corresponding supergraph's set.

The [[Complement of a Graph|complement of a given graph]] is a graph that shares the same vertices with such a graph, but has a disjoint set of edges.

# Digraphs

An [[Arc|arc]] is an edge that has a direction.

A graph whose edges are all directed (i.e. arcs) is called a [[Digraph|digraph]].

There are [[Types of Digraphs|many types of digraphs]] (🗺), among them:

- Similarly to a connected graph, a [[Connected Digraph|connected digraph]] is a digraph where a path (see below) exists between any two pair of vertices.

When we remove all the directions from a digraph $G$ that consists of all arcs, we get $G$'s [[Subjacent Graph|subjacent graph]].

# Vertices and Edges

## Vertices

Each vertex in a graph has an [[Open Neighbourhood|open]] and a [[Closed Neighbourhood|closed]] neighbourhood. A vertex where several edges incide is called a [[Multi-Edge|multi-edge]].

The amount of edges that incide on a vertex define its [[Vertex Degree|degree]].

In the context of a digraph, we can define a vertex's [[Internal and External Degrees of a Vertex|external and internal degrees]]. In this same context, we can have [[Types of Vertices in a Digraph|several types of vertices]], one of them being the [[Hanging Vertex|hanging vertex]].

The [[Length Between Vertices|length between two vertices]] is defined as the minimum amount of edges that must be traversed to reach one from the other. In the context of a connected graph, the [[Eccentricity|eccentricity]] of a vertex is defined as the length between that vertex and the farthest one in the graph.

## Edges

Edges with a direction are called [[Arc|arcs]].

Edges can be of [[Parallel Arcs|several types]].

# Operations with Graphs

Since graphs are essentially sets, we can define various operations on them:

- [[Union of Graphs|Union]], $\cup$
- [[Intersection of Graphs|Intersection]], $\cap$
- [[Sum of Graphs|Sum]], $+$
- [[Ring Sum of Graphs|Ring sum]], $\oplus$

We can additionally define [[Graph Fusion|graph fusion]] ($/$), a special operation that is carried out within one same graph, relative to one of its edges.

# Algorithms, Lemmas and Principles

By using the [[Havel-Hakimi Algorithm|Havel-Hakimi algorithm]], we can determine if a given non-increasing sequence of integers corresponds to the sequence of vertex degrees of a simple graph.

The [[Handshaking Lemma|Handshaking lemma]] tells us that given a graph with no edges, the sum of its vertices is always twice its number of edges.

The [[Pigeonhole Principle|Pigeonhole principle]] tells us that, given $n>m$, when we try to put $n$ objects in $m$ containers, then at least one container must be able to hold more than one object.

# Paths

A [[Path|path]] is an alternated finite sequence of vertices and degrees. Paths describe a "way" to traverse a graph.

The [[Length of a Path|length of a path]] is the number of edges in it. [[Path Concatenation|Path concatenation]] is the operation of joining two paths one after the other.

There are [[Types of Paths|various types of paths]], the most important of them being:

- A [[Simple Trajectory|simple trajectory]] is an open path with no repeated vertices or edges.

- A [[Circuit|circuit]] is a closed path with no repeated edges, just one repeated vertex.

All these three, paths, trajectories and circuits, can be directed, which obey the direction of the arcs they go through.

A [[Eulerian Path|Eulerian path]] is a path that contains all the edges in a graph exactly once.

# Trees

A [[Tree|tree]] is a connected graph with no circuits. A set of trees is called a [[Forest|forest]]. There are [[Types of Trees|various types of trees]].

In a tree, there can be various [[Leaf Vertex|leaf]] and [[Branch Vertex|branch]] vertices, but there can only be _just one_ [[Root Vertex|root vertex]] and _one_ [[Centre of a Tree|centre vertex]].

# Connectedness

An [[Articulation Point|articulation point]] is a vertex that when deleted disconnects a given connected graph. A [[Bridge|bridge]] is the equivalent concept for edges.

A [[Block|block]] is a connected graph that remains connected even after deleting any of its vertices.
