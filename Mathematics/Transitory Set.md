---
date: 2024-03-11
type: 🧠
tags:
  - MAC/6/PE
---

**Topics:** [[State Set]] - [[Stochastic Process]]

---

_**(definition)**_

Let $T$ be a subset of [[State Set|state set]] $S$ and let $T'$ be its [[Complement Set|complement]] in $S$. 

If each state in $T$ can be reached from any other in $T$, and it's possible to move from (at least) one state in $T$ to another in $T'$, then we call $T$ a **transitory set.

A **transitory state** is an element of a transitory set. A state that is not transitory is [[Ergodic Set|ergodic]]. 

In simpler terms, a transitory state is a state where there exists a probability of getting out of it, but then never coming back (i.e. when reaching an ergodic set). 

A [[Markov Chain|Markov chain]] may have no transitory states. Compare how a Markov chain must have at least one ergodic set.
