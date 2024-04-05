---
date: 2024-04-04
type: 🧠
tags:
  - MAC/6/PE
---

**Topics:** [[Transition Probabilities in a Markov Chain]] - [[Markov Chain]]

---

_**(definition)**_

Given a [[Markov Chain|Markov chain]] $\left\{ X_{t} \mid t \in \mathbb{N} \right\}$ and its [[One Step Transition Probability|one step transition probabilities]], if, for every $t, i, j$, we have that:

$$
\mathbb{P}(X_{t+1}=j \mid X_{t}=j) = \mathbb{P}(X_{1} = j \mid X_{0}=i)
$$

…then we say the one step transition probabilities are **stationary**. That is, the transition probabilities don't change across time and they are always the same.
