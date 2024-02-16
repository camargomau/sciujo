---
date: 2023-02-20
type: 🧠
tags:
  - MAC/S4/C4
---

**Topics:** [[Curve]] - [[Vector-Valued Function]]

---

_**(definition)**_

Let $r : \mathcal{D} \subseteq \mathbb{R} \to \mathbb{R}^n$ be a [[Vector-Valued Function|vector-valued function]].

Given an [[Arc Length Parameter|arc length parametrisation]], we define the _curvature_ of $r$ as:

$$
\kappa(s) := \left\| \frac{dT}{ds} \right\|
$$

…where $T$ is the [[Tangent Unit Vector|tangent unit vector]] in terms of the arc length parameter (that is, $T(s) = \frac{dr}{ds}$).

_**(theorem)**_

Given a non-[[Arc Length Parameter|arc length parametrisation]] $r(t)$ for a curve $c$, then the _curvature_ of $c$ is:

$$
\kappa(t) = \frac{\| T'(t) \|}{\| r'(t) \|}
$$
