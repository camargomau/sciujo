---
date: 2023-03-12
type: 🧠
tags:
  - MAC/S4/TG
---

**Topics:** [[Path]] - [[Graph Theory]]

---

There are several types of [[Path|paths]]:

- An _open path_ is a path that ends on a vertex different from the one that it starts on. A _closed path_ is the opposite: it starts and ends on the same vertex.

> [!example]-
> For example, given the graph:
>
> ![[Types of Paths-1.png]]
>
> We can have the following path from $V1$ to $V6$:
>
> $$
> V1, E3, V3, E10, V2, E2, V4, E11, V4, E7, V6
> $$

- A [[Simple Trajectory|simple trajectory]] is an open path with no repeated vertices or edges.

- A [[Circuit|circuit]] is a closed path with no repeated edges and just one repeated vertex (the start/end vertex).

- A _directed path_ is a path that respects the direction of the [[Arc|arcs]] it goes through.
