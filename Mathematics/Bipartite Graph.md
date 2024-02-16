---
date: 2023-02-23
type: 🧠
tags:
  - MAC/S4/TG
---

**Topics:** [[Graph]] - [[Graph Theory]]

---

_**(definition)**_

A _bipartite graph_ $G$ is a [[Graph|graph]] whose set of [[Vertex|vertices]] $V$ can be [[Partition of a Set|partitioned]] in two subsets $U$ and $W$, such that every [[Edge|edge]] of $G$ joins a vertex in $U$ and another one in $W$.

The pair $\{ U, W \}$ is called a _bipartition_ of $G$, and $U, W$ are called the _subsets of the bipartition_.

As the name suggests, a bipartite graph's partition only contains _two_ subsets.

> [!example]-
> The following graph is bipartite since $\{ U, W \} = \{ \{A, C\}, \{ B, D \} \}$ is a partition of $V$ that satisfies the necessary conditions.
>
> ![[Bipartite Graph-1.png|300]]

We can also have [[Complete Bipartite Graph|complete bipartite graphs]].

# Theorems

_**(theorem)**_

A bipartite graph can't have any [[Loop|loops]].

_**(theorem)**_

The smallest [[Simple Graph|simple graph]] that is not bipartite is the $K_3$ [[Complete Graph|complete graph]].
