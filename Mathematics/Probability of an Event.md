---
date: 2023-02-03
type: 🧠
tags:
  - MAC/4/PB
---

**Topics:** [[Probability]]

---

_**(definition)**_

In the Laplacian (classic) approach of probability, given $A \subset \Omega$ an [[Event|event]], the _probability_ of $A$ is defined as:

$$
\mathbb{P}(A) := \frac{|A|}{|\Omega|} = \frac{\text{favorable cases where $A$ occurs}}{\text{total cases}}
$$

> [!example]- Example
> Let $\varepsilon$ be "throw a die". Then $\Omega = \{ 1, 2, \dots, 6 \}$ ($|\Omega| = 6$).
>
> Let $A$ be "obtain an even number when the die is thrown". Then:
> - $A = \{ 2, 4, 6 \}$ ($|A| = 3$)
> - $\mathbb{P}(A) = \frac{|A|}{|\Omega|} = \frac{3}{6} = \frac{1}{2}$

# Geometrically

When trying to determine the probability of geometric events, then $|A|$ refers to the length/area/volume/etc. where $A$ occurs and $|\Omega|$ refers to the total length/area/volume/etc.

For example, let's say we throw a die on a [[Circle|circle]] of [[Radius|radius]] $r$. Let $A$ be "the die falls closer to the circle's centre point than to the circumference". Then:

$$
\mathbb{P}(A) = \frac{\pi\left(\frac{r}{2}\right)^2}{\pi r^2} = \frac{\pi \frac{r^2}{4}}{\pi r^2} = \frac{1}{4}
$$
