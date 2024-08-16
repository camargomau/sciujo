---
date: 2022-03-31
type: 🧠
tags:
  - MAC/2/GE
---

**Topics:** [[Geometry]] - [[Line]] - [[3D Space]]

---

Given two [[Line|lines]] in $\mathbb{R}^3$, we can have four different cases:

1. Both lines are the same line
2. Both lines are [[Parallel Lines|parallel]]
3. Both lines [[Line Intersection|intersect]] on a single [[point]]
4. Both lines never intersect, but one passes above the other

# Determining the Case

Given two lines in $\mathbb{R}^3$, $l_1 = \{ P + su\ :\ s \in \mathbb{R} \}$ and $l_2 = \{ Q + tv\ :\ t \in \mathbb{R} \}$, we can determine their specific case by calculating the following:

1. If $u \times v = 0$, $(P-Q) \times u = 0$, then $l_1 = l_2$
2. If $u \times v = 0$, $(P-Q) \times u \neq 0$, then $l_1$ and $l_2$ are parallel (but $l_1 \neq l_2$)
3. If $u \times v = 0$, $(P-Q) \cdot (u \times v) = 0$, then $l_1$ and $l_2$ intersect on a single point
4. If $(P-Q) \cdot (u \times v) \neq 0$, then $l_1$ and $l_2$ never intersect, but one passes above the other (we say they _cross_ each other)

We might find it convenient to check for the fourth condition first, then moving upwards, since we can reuse several of our calculations.
