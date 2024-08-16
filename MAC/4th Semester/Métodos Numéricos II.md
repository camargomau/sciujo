---
type: 🏫
tags:
  - MAC/4/MN2
---

# Interpolation

[[Interpolation]] is to estimate intermediate data points between other known points.

We can interpolate with various methods:

- Using a [[Taylor Polynomial|Taylor polynomial]], which approximates a complex function in a given interval.

- Using a [[Lagrange Polynomial|Lagrange polynomial]], which generalises the behaviour of a function when all we have is a discrete set of its points.

- [[Newton's Finite Differences Interpolation Method|Newton's finite differences interpolation method]], which also helps us obtain a polynomial that generalises the behaviour of a function given a discrete set of points, but is specifically used when the differences between the abscissas are constant.

- [[Newton's Divided Differences Interpolation Method|Newton's divided differences interpolation method]], which is very similar to Newton's finite differences method, but can work with points where the differences between the abscissas are non-constant.

- [[Hermite's Interpolation Method|Hermite's interpolation method]], which works very similarly to Newton's divided differences method, but uses derivatives to improve its accuracy.
