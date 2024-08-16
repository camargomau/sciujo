---
date: 2022-08-17
type: 🧠
tags:
  - MAC/3/C3
aliases:
  - open ball
---

**Topics:** [[Calculus]] - [[Topology]]

---

_**(definition)**_

We define the _open ball_ of radius $r \in \mathbb{R}$ around $x \in \mathbb{R}^n$ as:

$$
B_r(x)=\{ u \in \mathbb{R}^n \mid \| x - u \| < r \}
$$

> [!example]- Examples
> Take the following ball:
>
> $$
> B_1(0)\subseteq \mathbb{R} = \{ u \in \mathbb{R} \mid \|u-0\| < 1 \} = (-1, 1)
> $$
>
> This is a pretty easy to visualise ball that exists in $\mathbb{R}$, since it's just an open interval.
>
> Now take this other ball:
>
> $$
> B_{1}(0,0) = \{ (x, y) \in \mathbb{R}^{2}  \mid \|(x, y) - (0, 0) \| < 1 \} = \sqrt{x^{2}+y^{2}} < 1
> $$
>
> This ball is an open circle in $\mathbb{R}^{2}$ which is also rather easy to visualise. An analogue ball in $\mathbb{R}^{3}$ would be an open sphere.

Open balls are used for defining [[Interior Point|interior points]], [[Limit Point|limit points]] and the [[Limit of a Sequence|limit of a sequence]].
