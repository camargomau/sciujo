---
date: 2024-03-11
type: 🧠
tags:
  - MAC/6/PE
aliases:
  - "accessible"
---

**Topics:** [[Stochastic Process]]

---

_**(definition)**_

Given a [[Markov Chain|Markov chain]], we say that the [[State Set|state]] $j$ is _accessible_ from the state $i$ if $p_{ij}^{(n)} > 0$ for some $n \geq 0$.

Do note that we can have the case of **not** having the state $i$ being accessible from the state $j$, but having the state $j$ accessible from $i$. 

When both cases are satisfied (i.e. $i$ accessible from $j$, and $j$ accessible from $i$), we say that **both states communicate**. 

We can [[Partition of a Set|partition]] the set of states in a given chain by grouping them into [[Markov Chain State Class|classes]], each one containing states that _all_ communicate. 

# Properties

- Every state communicates with itself (since $p_{ii}^{(0)} = 1$; [[Properties of Relations|reflexive]]).
- If $i$ communicates with $j$, then $j$ communicates with $i$ ([[Properties of Relations|symmetric]]).
- If $i$ communicates with $j$, and $j$ communicates with $k$, then $i$ communicates with $k$ ([[Properties of Relations|transitive]]).
