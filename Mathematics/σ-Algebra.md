---
date: 2023-02-08
type: 🧠
tags:
  - MAC/S4/PB
aliases:
  - sigma-algebra
  - σ-algebra
---

**Topics:** [[Probability]]

---

_**(definition)**_

A _$\sigma$-algebra_ (_sigma-algebra_), denoted $\mathscr{F}$, is a family of subsets of one same [[Sample Space|sample space]] $\Omega$ such that:

1. $\Omega \in \mathscr{F}$
2. If $A \in \mathscr{F} \implies A^c \in \mathscr{F}$
3. If $(A_n)_{n \geq 1}$ is a collection of subsets in $\mathscr{F}$, then $\bigcup_{n=1}^\infty A_n \in \mathscr{F}$

> [!example]-
> Let's toss a coin.
>
> $$
> \Omega = \{ X, C \}
> $$
>
> Is $\mathscr{F} = \mathcal{P}(\Omega)$ ([[Power Set|power set]]) a $\sigma$-algebra?
>
> Let's see what we have:
>
> 1. $\Omega \in \mathscr{F}$
> 2. We check each subset and its complement:
> 	- $\varnothing \in \mathscr{F} \land \varnothing^c = \Omega \in \mathscr{F}$
> 	- $\Omega \in \mathscr{F} \land \Omega^c = \varnothing \in \mathscr{F}$
> 	- $X \in \mathscr{F} \land X^c = C \in \mathscr{F}$
> 	- $C \in \mathscr{F} \land C^c = X \in \mathscr{F}$
>  1. We check every possible union:
> 	 - $\varnothing \cup \Omega = \Omega \in \mathscr{F}$
> 	 - $\Omega \cup C = \Omega \in \mathscr{F}$
> 	 - $C \cup X \cup \varnothing = \Omega \in \mathscr{F}$
> 	 - $X \cup \Omega \cup \varnothing \cup C = \Omega \in \mathscr{F}$
> 	 - etc.
>
> Since the three axioms are satisfied, **$\mathscr{F} = \mathcal{P}(\Omega)$ is a $\sigma$-algebra**.
