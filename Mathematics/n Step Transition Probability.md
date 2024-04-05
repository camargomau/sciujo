---
date: 2024-04-04
type: 🧠
tags:
  - MAC/6/PE
---

**Topics:** [[Transition Probabilities in a Markov Chain]] - [[Markov Chain]]

---

_**(theorem)**_

In a [[Markov Chain|Markov chain]], the existence of [[One Step Transition Probability|one step]] [[Stationary Transition Probability|stationary transition probabilities]] implies that for every $i, j$ and $n \in \mathbb{N}$:

$$
\mathbb{P}(X_{t+n}=j \mid X_{t}=i) = \mathbb{P}(X_{n}=j\mid X_{0}=i)
$$

We call these the **$n$ step transition probabilities**.

It can be handy to write these probabilities in a [[Transition Matrix|transition matrix]].

# Simpler Notation

To simplify notation, we'll agree on:

$$
\begin{align}
p_{ij} &= \mathbb{P}(X_{t+1}=j \mid X_{t} = i) \\[0.5em]
p_{ij}^{(n)} &= \mathbb{P}(X_{t+n}=j \mid X_{t} = i)
\end{align}
$$

Note that when $n = 1$, then $p_{ij}^{(n)} = p_{ij}$. 

Observe that, when $n=0$, we have $p_{ij}^{(n)} = \mathbb{P}(X_{0} = j \mid X_{0} = i)$, which is trivially $1$ when $i = j$ and $0$ otherwise.

# Properties

_**(theorem)**_

Derived from the properties of a [[Probability Measure|probability measure]], we have that:

- $p_{ij}^{(n)} \geq 0$, for every $i,j$ and $n=0,1,2,\dots$
- $\sum\limits_{j=0}^{s} p_{ij}^{(n)}=1$, for every $i$ and $n = 0,1,2,\dots$
