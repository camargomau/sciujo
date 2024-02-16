---
date: 2023-04-11
type: 🧠
---

**Topics:** [[Graph Theory]]

---

In a [[Connected Graph|connected graph]], the _eccentricity_ of a [[Vertex|vertex]] $v_i$ is the [[Length Between Vertices|length]] between $v_i$ and the farthest $v_j$.

That is:

$$
E(v_i)  = \max\{d(v_i, v_j) \mid v_i, v_j \in G\}
$$

# Centre of a Tree

The concept of eccentricity is useful when we're trying to identify the _[[Centre of a Tree|centre of a tree]]_ $c$, since:

$$
E(c) = \min\{E(v_i)\}
$$
