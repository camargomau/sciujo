---
date: 2022-05-02
type: 🧠
tags:
  - MAC/S2/C2
---

**Topics:** [[Calculus]] - [[Sequence]]

---

_**(definition)**_

Let $\{a_n\}_{n \in \mathbb{N}} \subseteq \mathbb{R}$ be a [[Sequence|sequence]].

We define the _partial sum sequence_ of $\{a_n\}$ as:

$$
\left\{ S_n \right\} = \left\{ \sum_{i=1}^n a_i \right\}_{n \in \mathbb{N}}
$$

If this sequence [[Limit of a Sequence|converges]], then we say that the _series_ $\sum_{n = 1}^\infty a_n$ converges and that $\sum_{n = 1}^\infty a_n = \lim_{n \to \infty} S_n$.

> [!example]-
>
> Let $\{a_n\} = \left\{ \frac{1}{2^{n-1}} \right\}$. It's clear that:
>
> - $a_1 = 1$
> - $a_2 = \frac{1}{2}$
> - $a_3 = \frac{1}{2^2}$
> - $a_4 = \frac{1}{2^3}$
> - etc.
>
> Its partial sum sequence $\{ S_n \}$ gives us:
>
> - $S_1 = 1$
> - $S_2 = 1 + \frac{1}{2}$
> - $S_3 = 1 + \frac{1}{2} + \frac{1}{2^2}$
> - $S_4 = 1 + \frac{1}{2} + \frac{1}{2^2} + \frac{1}{2^3}$
> - $\vdots$
> - $S_n = 1 + \frac{1}{2} + \frac{1}{2^2} + \frac{1}{2^3} + \dots + \frac{1}{2^{n-1}}$
>
> …so it becomes clear that:
>
> $$
> \{ S_n \} = \left\{ \sum_{i=1}^n \frac{1}{2^{n-1}} \right\}
> $$
>
> …which we can rewrite as:
>
> $$
> \{ S_n \} = \left\{ \frac{1 - \frac{1}{2^n}}{1 - \frac{1}{2}} \right\} = \left\{ 2 - \frac{1}{2^{n-1}} \right\}
> $$
>
> Then, by calculating the [[Limit of a Sequence|limit]] of the partial sum sequence:
>
> $$
> \lim_{n \to \infty} S_n = 2
> $$
>
> …we can obtain the concrete value to which the series converges:
>
> $$
> \sum_{n=1}^\infty \frac{1}{2^{n-1}} = 2
> $$

The convergence of series can be tested with [[Convergence Tests for Series|several methods]].
