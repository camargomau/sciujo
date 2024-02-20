---
date: 2024-02-01
type: 🧠
tags:
  - MAC/6D
---

**Topics:** [[Integral Transform]]

---

An **integral transform** is an [[Operator|operator]] that is derived from other [[Function|functions]] though a [[Definite Integral|definite integral]]. They allow us to switch from a reference system to another, with the advantage of being able to go back to the original system (this ability being the inverse transform).

Instances of integral transforms include the [[Laplace Transform|Laplace transform]].

_**(definition)**_

Formally, an **integral transform** is an operator that associates a new function to a given [[Set|set]] through integration with respect to a given parameter:

$$
T\{f(t)\} = F(s) = \int_{a}^{b} K(t,s) f(t) \ dt 
$$

…where:

- $K(t,s)$ is the _integral kernel_ of the transform
- $(a,b)$ is the interval that is commonly infinite
- $F(s)$ is the _transform_ of the function $f$

Do note that integral transforms are [[Linear Transformation|linear transformations]]. 