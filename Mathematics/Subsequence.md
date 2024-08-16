---
date: 2022-04-29
type: 🧠
tags:
  - MAC/2/C2
aliases:
  - subsequence
---

**Topics:** [[Calculus]] - [[Sequence]]

---

_**(definition)**_

Let $\{ a_n \} \subseteq \mathbb{R}$ be a [[Sequence|sequence]].

We say that $\{ b_n \}$ is a _subsequence_ of $\{ a_n \}$ if $\forall\ s \in \mathbb{N}$, $\exists\ n \in \mathbb{N}$ such that $b_s = a_n$.

Further more, the order of the sequence $\{ a_n \}$ is inherited.

_**(lemma)**_ ^7e744c

All sequences $\{ a_n \}$ contain a [[Increasing and Decreasing Sequence|monotone]] subsequence.

# Bolzano's Theorem

_**(theorem)**_

Let $\{ a_n \}_{n \in \mathbb{N}}$ be a [[Bound|bounded]] [[Sequence|sequence]], then $\{ a_n \}$ has a convergent [[Subsequence|subsequence]].

> [!abstract]- Proof
> From [[Subsequence#^7e744c|a specific lemma]], we know that $\exists\ \{ b_n \}_{n \in \mathbb{N}}$, a [[Increasing and Decreasing Sequence|monotone]] [[Subsequence|subsequence]] of $\{ a_n \}$, that is [[Bound|bounded]].
>
> $\{ b_n \}$ being a bounded monotone sequence implies it [[Limit of a Sequence#^b44b3b|converges]].
