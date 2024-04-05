---
date: 2024-03-15
type: 🧠
tags:
  - MAC/6/PE
---

**Topics:** [[Markov Chain]] - [[Stochastic Process]]

---

_**(definition)**_

In the context of a [[Markov Chain|Markov chain]], the **recurrence time** is the minimum amount of steps that are needed to _go back_ to a given [[State Set|state]] _for the first time_. 

Compare the [[First-Passage Time|first-passage time]], which refers to the minimum amount of steps that are needed to get to a state (for the first time, too).

The recurrence time to a state $i$, denoted $\mu_{ii}$ (similarly to a first-passage time), is given by:

$$
\mu_{ii} = \frac{1}{\pi_{i}}
$$

…where $\pi_{i}$ is the [[Steady State Probability|steady state probability]] of $i$.
