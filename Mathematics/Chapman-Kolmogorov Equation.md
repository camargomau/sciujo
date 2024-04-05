---
date: 2024-04-04
type: 🧠
tags:
  - MAC/6/PE
---

**Topics:** [[Markov Chain]] - [[Transition Matrix]] - [[Transition Probabilities in a Markov Chain]]

---

_**(theorem)**_

Given a [[Markov Chain|Markov chain]], we can obtain its [[Transition Probabilities in a Markov Chain|transition probabilities]] with the **Chapman-Kolmogorov equation**. 

To obtain [[n Step Transition Probability|n step transition probabilities]]:

$$
p_{ij}^{(n)} = \sum\limits_{k=0}^{s} p_{ik}^{(m)} p_{kj}^{(n-m)} 
$$

…for every $i,j,n$ and $0 \leq m \leq n$.

> [!question]- Explanation
> This equation is derived from the fact that we can calculate the probability of going from the state $i$ to the state $j$ by:
> 
> - Calculating the probability of going from $i$ to another intermediate state $k$ in $m$ steps ($m \leq n$)
> - Calculating the probability of going from that other intermediate state $k$ to $j$ in $n-m$ steps
> - [[Multiplication Principle|Multiplying]] these two probabilities so that we obtain the probability of both happening
> - [[Addition Principle|Adding up]] all these probabilities for every possible $k$
