---
date: 2022-04-27
type: 🧠
tags:
  - MAC/2/C2
aliases:
  - Monotone Sequence
  - monotone sequence
  - Increasing Sequence
  - increasing sequence
  - Decreasing Sequence
  - decreasing sequence
  - increasing and decreasing sequences
---

**Topics:** [[Calculus]] - [[Sequence]]

---

_**(definition)**_

Let $\{ a_n \}_{n \in \mathbb{N}}$ be a [[Sequence|sequence]].

We say that this sequence is _strictly increasing_ if for $s>t \implies a_s > a_t$. Similarly, we say that it is decreasing if for $s > t \implies a_s < a_t$.

On the other hand, we say that the sequence is _increasing_ or _non-decreasing_ if for $s>t \implies a_s \geq a_t$. Similarly, we say that it is _decreasing_ or _non-increasing_ if for $s > t \implies a_s \leq a_t$.

Increasing or decreasing sequences are called _monotone sequences_.

# Bounds and Convergence

_**(theorem)**_

If $\{ a_n \}$ is a [[Bound|bounded]] monotone sequence, then $\{ a_n \}$ converges.

> [!abstract]- Proof
> Without loss of generality, let's suppose that $\{ a_n \}$ is increasing.
>
> Since $\{ a_n \}$ is bounded, then $\exists\ \alpha \in \mathbb{R}$ such that $\alpha = \sup\{ x \in \mathbb{R} | x = a_n \} = \sup(A)$.
>
> Let $\varepsilon > 0$. Since $\alpha$ is the [[Supremum|supremum]], then $\exists\ a_N \in A$ such that $\alpha - a_N < \varepsilon$.
>
> Since the sequence is increasing, then $\forall m > N$:
>
> $$
> \begin{align} a_m &> a_n \\ -a_m &< -a_n \\ \alpha - a_m &< \alpha - a_N < \varepsilon \\ | \alpha - a_m | &< \varepsilon \end{align}
> $$
>
> With transitivity, we get that:
>
> $$
> a_m > a_n \implies | \alpha - a_m | < \varepsilon \text{ if } m > N
> $$
>
