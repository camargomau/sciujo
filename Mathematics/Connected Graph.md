---
date: 2023-02-23
type: 🧠
tags:
  - MAC/S4/TG
---

**Topics:** [[Graph Theory]] - [[Graph]]

---

_**(definition)**_

A [[Graph|graph]] $G$ is said to be _connected_ if we can reach any given [[Vertex|vertex]] from any other one.

That is, a graph is connected if there is an [[Edge|edge]] between any two vertices. In any other case, we say that $G$ is _disconnected_.

We can also have [[Strongly Connected Graph|strongly connected graphs]].

# Components

_**(theorem)**_

A graphic is disconnected if and only if its set of vertices can be divided into 2 or more non-empty [[Disjoint Set|disjoint]] sets, such that there are no edges that start in one of the subsets and end in another one.

We call each of these subsets _components_.

# Two Odd Degrees

_**(theorem)**_

If a graph has _exactly_ two vertices of odd [[Vertex Degree|degree]], then there exists a [[Simple Trajectory|trajectory]] that joins them together.

In such a case, the graph is connected.
