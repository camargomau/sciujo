---
date: 2022-08-15
type: 🧠
tags:
  - MAC/3/C3
aliases:
  - metric space
  - Metric
  - metric
---

**Topics:** [[Calculus]]

---

_**(definition)**_

Let $X$ be a [[set]] and $d : x \times x \to \mathbb{R}$ be a [[Function|function]]. We say that $(X, d)$ is a _metric space_ if:

1. $d(x, y) = 0 \iff x = y$
2. $d(x, y) = d(y, x)$, $\forall x, y \in X$
3. $d(x, z) \leq d(x, y) + d(y, z)$, $\forall x, y, z \in X$

In such a case, we say that $d$ is a _metric_.

> [!tip]- Concept of Distance
> Notice that these properties are related to the concept of distance. The first one asks for any two same elements to be in the same place, the second one asks for the distance to be the same between any two elements regardless of order, and the third one is the [[Triangle Inequality|triangle inequality]].

# Examples

> [!example]+ Distance in $\mathbb{R}^n$
> In $\mathbb{R}^n$, we define the distance (metric) as:
>
> $$
> d(x, y) = \| x-y \|
> $$
>
> That is, the [[Norm under Real Numbers|norm]] of the difference between $x$ and $y$.

> [!example]- Example 1
> Let $X = \{a_1, a_2, a_3, a_4, a_5\}$ and $d : x \times x \to \mathbb{R}$ be given by:
>
> $$
> d(a_i, a_j) = \begin{cases} 1\text{ if }i \neq j \\ 0\text{ if }i = j \end{cases}
> $$
>
> This $d$ defines a metric (it satisfies the previous properties).

> [!example]- Example 2
> $(\mathbb{R}, d)$ where $d : \mathbb{R} \times \mathbb{R} \to \mathbb{R}$, $d(x, y) = | x - y |$.
>
> The properties of a metric space are satisfied, since they follow the properties of the [[absolute value]].

> [!example]- Example 3
> Let $\mathcal{C}[0, 1] = \{ f : [0, 1] \to \mathbb{R} \mid f\text{ is continuous} \}$ and $d : \mathcal{C}[0, 1] \times \mathcal{C}[0, 1] \to \mathbb{R}$ be given by:
>
> $$
> d(f, g) = \sup \{ |f(x) - g(x)|\ \big|\ x \in [0, 1] \}
> $$
>
> $d$ is a metric.
>
