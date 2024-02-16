---
date: 2023-04-16
type: 🧠
tags:
  - MAC/S4/C4
---

**Topics:** [[Path Integral]] - [[Calculus]]

---

[[Path Integral|Path integrals]] can be used for many applications. Apart from the obvious use for calculating the area of a surface, there are many others such as calculating the average of a function over a curve or calculating the centre of mass given a density function.

# Average of a Function

Let $f : \mathbb{R}^n \to \mathbb{R}$ be a [[Function|function]] and let $c$ be a curve in $\mathbb{R}^n$ parametrised by $r:[a,b] \to \mathbb{R}^n$.

The _average_ of $f$ over $c$, denoted $\mu_{f}$ is given by:

$$
\mu_f = \frac{\int_c f\ ds}{\int_a^b \| c'(t) \| \ dt}
$$

Note that the denominator is just the [[Arc Length|arc length]] of $c$.

# Centre of Mass

Let $\rho:\mathbb{R}^{3} \to \mathbb{R}$ be a function that defines the density of an object in any one of its points. Let $c$ be a curve that defines the points where the object exists.

The _total mass_ of the object defined by $c$ is given by:

$$
M_{t} = \int_{c} \rho(x,y,z) \, ds
$$

The coordinates of its _[[Centre of Mass|centre of mass]]_ are given by:

$$
\mathbf{C_{m}} = \frac{1}{M_{t}}\left( \int_{c} \rho(x,y,z) \ x \ ds, \int_{c} \rho(x,y,z) \ y \ ds, \int_{c} \rho(x,y,z) \ z \ ds \right)
$$
