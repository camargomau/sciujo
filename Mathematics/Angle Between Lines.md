---
date: 2022-04-19
type: 🧠
tags:
  - MAC/S2/GE
---

**Topics:** [[Geometry]] - [[Line]] - [[Angle]]

---

Given two [[Line|lines]] in $\mathbb{R}^3$, $l_1 = \{ P + su\ :\ s \in \mathbb{R} \}$ and $l_2 = \{ Q + tv\ :\ t \in \mathbb{R} \}$, we can determine the angle between them with:

$$
\cos \theta = \frac{|u \cdot v|}{\|u\| \|v\|}
$$

The angle $\theta$ between any two lines will always be such that $0 \leq \theta \leq \frac{\pi}{2}$.

> [!hint]- Comparing formulas
> Notice this formula is almost the same as the formula for the [[Angle Between Vectors]], the only difference being the fact that we take the absolute value of $u \cdot v$.
>
> This is because two vectors of equal magnitude but opposite directions generate the same exact line (given an adequate starting point).

# Orthogonality

These two lines $l_1$ and $l_2$ are [[orthogonal]] if and only if their direction vectors $u$ and $v$ are orthogonal.

That is, two lines are orthogonal if and only if their angle $\theta = \frac{\pi}{2}$ (in other words, if $\cos \theta = 0$).

# Parallelism

These two lines $l_1$ and $l_2$ are parallel if and only if their direction vectors are parallel.

That is, two lines are parallel if and only if their angle $\theta = 0$ (in other words, if $\cos \theta = 1)$.
