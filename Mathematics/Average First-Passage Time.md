---
date: 2024-04-04
type: 🧠
tags:
  - MAC/6/PE
---

**Topics:** [[First-Passage Time]]

---

_**(theorem)**_

In a [[Markov Chain|Markov chain]], we can calculate the **average [[First-Passage Time|first-passage time]]** for the state $j$ when starting at $i$, denoted $p_{ij}$, with:

$$
\mu_{ij} = 1 + \sum_{k\neq j} p_{ik}\ \mu_{kj}
$$

> [!tip]- Explanation
> Here, we are basically considering that the only two possibilities for the first transition are two:
> 
> 1. Reaching $j$
> 2. Reaching any other $k \neq j$
> 
> If we reach $j$ during the first transition, then it only took us 1 step to reach it.
> 
> If we first pass through $k \neq j$ before eventually reaching $j$, then we have to take 1 step (to reach $k$) then take $\mu_{kj}$ more steps to reach $j$ from $k$. 
> 
> When taking into consideration the probabilities of reaching through any $k$ and adding up all of them, we obtain the average first-passage time from $i$ to $j$.
