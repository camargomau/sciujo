---
date: 2022-05-12
type: 🧠
tags:
  - MAC/2/GE
---

**Topics:** [[Geometry]] - [[3D Space]] - [[Plane]] - [[Angle]]

---

_**(theorem)**_

The angle $\theta$ between two [[Plane|planes]] $\Pi_1$ and $\Pi_2$ with their respective equations…

$$
\Pi_1: Ax + B1 y + Cz + D = 0
$$

$$
\Pi_2 : A'x + B'y + C'z + D' = 0
$$

…is determined by the equality:

$$
\cos \theta = \frac{ | AA' + BB' + CC' | }{\sqrt{A^2 + B^2 + C^2}\ \sqrt{(A')^2 + (B')^2 + (C')^2}}
$$

Given the respective [[Normal Vector|normal vectors]], we can rewrite this equality as:

$$
\cos \theta = \frac{ | n_1 \cdot n_2 | }{\| n_1 \| \| n_2 \| }
$$

Notice the formula is very similar to the one used to obtain the [[Angle Between Lines|angle between lines]].

# Criterium

- The planes $\Pi_1$ and $\Pi_2$ are [[parallel]] if and only if there exists a real number $k \neq 0$ such that:

$$
A = kA', \quad B = kB', \quad C = kC'
$$

- The planes $\Pi_1$ and $\Pi_2$ are the same plane if they're parallel and if $D = kD'$.

- The planes $\Pi_1$ and $\Pi_2$ are [[Orthogonal|orthogonal]] if and only if $AA' + BB' + CC' = 0$ (i.e. if $n_1 \cdot n_2 = 0$).
