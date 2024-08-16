---
date: 2022-05-17
type: 🧠
tags:
  - MAC/2/GE
---

**Topics:** [[Geometry]] - [[3D Space]] - [[Plane]]

---

Given two [[Plane|planes]] in $\mathbb{R}^3$ we can find the line where they intersect by:

1. Finding their [[Normal Vector|normal vectors]] and calculating the cross product between them
2. Finding a common [[point]] between them (we can find such a point by giving a variable a concrete value, then solving the resulting equation system)
3. Building a line with such a point and vector

In general, let:

$$
\Pi_1 = Ax + By + Cz + D = 0
$$

$$
\Pi_2 = Ex + Fx + Gx + H = 0
$$

…be the equations for two planes $\Pi_1$ and $\Pi_2$ in $\mathbb{R}^3$. Then, the intersection line for these planes is:

$$
l = \{ P + t(n_1 \times n_2) : t \in \mathbb{R} \}
$$

…where $P$ is a common point between the planes, and $n_1$ and $n_2$ are the normal vectors for each respective plane.
