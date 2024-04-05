---
date: 2024-03-20
type: 🧠
tags:
  - MAC/6/PE
---

**Topics:** [[Markov Chain]] - [[Absorbing Set]]

---

_**(definition)**_

In a [[Markov Chain|Markov chain]], given a $k$ an [[Absorbing Set|absorbing state]], the probability of reaching $k$ when we start from another state $i$ is called the **probability of absorption to $k$**. This probability is denoted by $f_{ik}$.

_**(theorem)**_

The probability of absorption to $k$ when starting at $i$ is given by:

$$
f_{ik} = \sum_{j=0} p_{ij} f_{jk}
$$

…where $f_{kk} = 1$.

_**(theorem)**_

Let $k_{1}, k_{2}, \dots, k_{s}$ be all absorbing states in a Markov chain. Then, for a fixed state $i$, it follows that:

$$
\sum_{c=1}^{s} f_{ik_{c}} = 1
$$

In other words, the result of adding up all possible absorption probabilities when starting at a given state $i$ is simply $1$.

_**(observation)**_

Note that we'll have $f_{ik}=0$ if the state $i$ is absorbing and different from $k$.


