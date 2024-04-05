---
date: 2024-04-04
type: 🧠
tags:
  - MAC/N/PE
---

**Topics:** [[Markov Chain]] - [[Transition Probabilities in a Markov Chain]]

---

_**(theorem)**_

The usual [[Transition Probabilities in a Markov Chain|transition probabilities]] in a [[Markov Chain|Markov chain]] are actually [[Conditional Probability|conditional]] in the sense that they consider a specific present state. For instance, in the case of [[One Step Transition Probability|one step transition probabilities]], they are $\mathbb{P}\left( X_{n} = j \mid X_{t} = i \right)$.

If we want to obtain the **_unconditional_ transition probabilities**, then we can use the [[Initial Probability Vector|initial probability vector]] $a = \left( a_{0}, a_{1}, \dots, a_{n} \right)$ to calculate:

$$
\mathbb{P}\left( X_{n} = j \right) = a_{0} p_{0j}^{(n)} + a_{1} p_{1j}^{(n)} + \dots + a_{m} p_{mj}^{(n)}
$$
