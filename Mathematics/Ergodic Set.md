---
date: 2024-03-11
type: 🧠
tags:
  - MAC/6/PE
aliases:
  - ergodic state
---

**Topics:** [[State Set]] - [[Stochastic Process]]

---

_**(definition)**_

Given a [[Markov Chain|Markov chain]], let $E$ be a subset of its [[State Set|state set]] $S$ and let $E'$ be its [[Complement Set|complement]] in $S$.

If each state in $E$ can be reached from any other state in $E$, but no state in $E'$ can be reached from any in $E$, then we say that $E$ is an **ergodic set** (or _recurrent set_). 

Thus, in a given ergodic set, all states [[State Communication|communicate]] with each other. Once an ergodic set has been reached, it's no longer possible to get out of it, but it  is still possible to move across the states in that set. 

An **ergodic state** is an element of an ergodic set. A state that is not ergodic is [[Transitory Set|transitory]]. An ergodic set with a single element is said to be [[Absorbing Set|absorbing]]. 

Every finite [[Markov Chain|Markov chain]] has at least one ergodic set, but there can be more. Compare how a Markov chain may have no transitory states. 
