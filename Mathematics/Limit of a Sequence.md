---
date: 2022-04-27
type: 🧠
tags:
  - MAC/S2/C2
aliases:
  - convergent sequence
  - convergent sequences
---

**Topics:** [[Calculus]] - [[Sequence]] - [[Limit]]

---

_**(definition)**_

Let $\{ a_n \}_{n \in \mathbb{N}} \subset \mathbb{R}$ be a [[Sequence|sequence]] and $L \in \mathbb{R}$.

We say that $L$ is the _limit of_ $\{ a_n \}_{n \in \mathbb{N}}$ when $n$ tends to [[infinity]] if $\forall\ \varepsilon > 0$, $\exists\ N \in \mathbb{N}$ such that $| a_m - L | < \varepsilon$ if $m > N$.

This is denoted by:

$$
\lim_{n \to \infty} a_n = L
$$

> [!abstract]- Proof
> Let $\varepsilon > 0$.
>
> The [[Archimedian Property]] tells us that $\exists N \in \mathbb{N}$ such that $\frac{1}{N} < \varepsilon$.
>
> With that, if $m > N$, then:
>
> $$
> \frac{1}{m} < \frac{1}{N}
> $$
>
> Finally, we can see that:
>
> $$
> \left| \frac{1}{m} - 0 \right| < \left| \frac{1}{N} - 0 \right| < \varepsilon
> $$

> [!quote]- Definition in terms of an [[Open Ball|open ball]]
> We say that $L$ is the limit of $\{a_{k}\}$ if $\forall \varepsilon > 0$, $\exists N \in \mathbb{N}$ such that $a_{m}\in B_\varepsilon(L)$ $\forall m > N$.
>
> This is the same definition as above, but given in terms of an open ball.

When a sequence has a limit, we say that it _converges_. When it doesn't, then we say it _diverges_. ^b44b3b

Limits of sequences can be [[Operations of Limits of Sequences|operated]].

# Limit of a Sum of Sequences

_**(theorem)**_

Let $\{ a_n \}, \{ b_n \} \subseteq \mathbb{R}$ be sequences such that $\lim_{n \to \infty} a_n = A$ and $\lim_{n \to \infty} b_n = B$.

Then, the sequence $\{ c_n \} = \{ a_n + b_n \}$ converges and $\lim_{n \to \infty} c_n = A + B$.

# Limit of a Sequence Greater than 0

_**(theorem)**_

If $a_n \geq 0$ $\forall\ n \in \mathbb{N}$ and $\{ a_n \}_{n \in \mathbb{N}}$ is convergent, then:

$$
\lim_{n \to \infty} a_n \geq 0
$$

# Sandwich Limit

_**(theorem)**_

If $\{ a_n \}_{n \in \mathbb{N}}$, $\{ b_n \}_{n \in \mathbb{N}}$, $\{ c_n \}_{n \in \mathbb{N}}$ are convergent sequences such that:

$$
a_n \leq b_n \leq c_n\quad \forall\ n \in \mathbb{N}
$$
Then:

$$
\lim_{n \to \infty} a_n \leq \lim_{n \to \infty} b_n \leq \lim_{n \to \infty} c_n
$$

_(we can prove this theorem with the previous theroem)_
