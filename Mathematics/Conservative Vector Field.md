---
date: 2023-04-12
type: 🧠
tags:
  - MAC/S4/C4
---

**Topics:** [[Vector Field]]

---

_**(definition)**_

A _conservative vector field_ is a [[Vector Field|vector field]] that has one (or several) [[Potential Function|potential functions]].

All conservative fields are [[Curl of a Vector Field|irrotational]] (i.e. their curl is $0$).

# Line Integral

## Path Independence

_**(theorem)**_

The [[Line Integral|line integral]] of a conservative vector field is _path-independent_.

That means that given a conservative vector field $F$, its line integral will **only depend on the endpoints** of the path, _regardless of the actual path_ chosen. That is, if $P_{1}$ and $P_{2}$ are _any_ two paths that have the _same endpoints_:

$$
\int_{P_{1}} F \cdot ds = \int_{P_{2}} F \cdot ds
$$

_**(theorem)**_

The above expression is equivalent to:

$$
\int_{P_{c}} F \cdot ds = 0
$$

…where $P_{c}$ is a closed path (i.e. its endpoints are one same point).

## Fundamental Theorem of Calculus for Line Integrals

_**(theorem)**_

Given $F$ a conservative vector field on a region $R \subseteq \mathbb{R}^3$, then [[Line Integral|the integral of]] $F$ on a [[Curve|curve]] in $R$ is equal to:

$$
\int_c F \cdot ds = f(B) - f(A)
$$

…where $f$ is a [[Potential Function|potential function]] of $F$, and $A$ and $B$ are the extreme points of the curve.

Notice that this is basically the [[Fundamental Theorem of Calculus|fundamental theorem of calculus]] for line integrals.
