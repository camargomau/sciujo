---
date: 2024-05-18
type: 🧠
tags:
  - MAC/6/PE
---

**Topics:** [[Policy Improvement Method for MDPs]] - [[Markov Decision Process]]

---

_**(theorem)**_

In the context of an [[Markov Decision Process|MDP]], the **expected long term cost for a given [[Markov Decision Process Policy|policy]] $r$** can be expressed as:

$$
g\{r\} = \sum_{i=0}^{m} \pi_{i}\ C_{ik}
$$

…where $\pi_{i}$ denotes the [[Steady State Probability|steady state probability]] of the state $i$. 

**Do not forget** that the policy $r$ defines which decision $k$ is made in which state $i$.
