---
date: 2022-08-17
type: 🧠
tags:
  - MAC/3/C3
---

**Topics:** [[Calculus]] - [[Topology]]

---

_**(definition)**_

Let $x \in A \subseteq \mathbb{R}$. We say that $x$ is an _interior point_ of $A$ if $\exists \delta \in \mathbb{R}^+$ such that $B_{\delta}(x) \subseteq A$ (the [[Open Ball|open ball]]).

In other words, $x$ is an interior point if we can form an open ball such that _all_ of the ball is contained within $A$.

The set of interior points of $A$ is called the _interior_ of $A$, written $\text{int}(A)$.

> [!example]-
>
> Let $A = [-1, 1]$.
>
> - $x = 0$ is an interior point, since $\delta \in [0, 1]$ yields a ball that's contained in $A$.
> - $x = -1$ is not an interior point, since there's no $\delta$ such that the resulting ball is contained in $A$.

If $A = \text{int}(A)$, then $A$ is an [[Open Set|open set]].
