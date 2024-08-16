---
date: 2023-02-08
type: 🧠
tags:
  - MAC/4/PB
aliases:
  - "probability function"
---

**Topics:** [[Probability]]

---

_**(definition)**_

A _probability measure_ (or _probability function_ or simply _probability_) is a [[Function|function]] $\mathbb{P} : \mathscr{F} \to [0,1]$ ($\mathscr{F}$ a [[σ-Algebra|σ-algebra]]) such that:

1. $\mathbb{P}(A) \geq 0$ (non-negative)
2. $\mathbb{P}(\Omega) = 1$
3. If $(A_n)_{n \geq 1} \in \mathscr{F}$ such that $A_i \cap A_j = \varnothing$ ($i \neq j$), then:

$$
\mathbb{P}\left( \bigcup_{n=1}^\infty A_n \right) = \sum_{n=1}^\infty \mathbb{P}(A_n)
$$

Probability measures have [[Properties of a Probability Measure|specific properties]].
