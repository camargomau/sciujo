---
date: 2024-05-18
type: 🧠
tags:
  - MAC/6/PE
---

**Topics:** [[Markov Decision Process]]

---

Given an [[Markov Decision Process|MDP]], we can obtain an _approximation_ to the optimal [[Markov Decision Process Policy|policy]] by using the **successive approximations method**. 

The basic idea behind this method is to find an optimal policy for the process when only $n$ periods remain, starting from $n=1$ (one period away from finishing) and continuing onwards. As $n$ grows, the optimal policies that are found converge to the optimal policy for the MDP (i.e. the optimal policy when "infinite" periods remain). Thus, the optimal policies that are found for each $n$ are **successive approximations** to the optimal policy.

This method mainly uses the [[Expected Total Cost of an MDP Starting from a State|expected total costs starting from a state]] $V_{i}^n$, though we'll be using the ones that correspond to the optimal policy among all the possible ones, instead of just the ones for a given [[Markov Decision Process Policy|policy]]. 

# Algorithm

Evidently, the method is iterative. We will iterate over $n$, the amount of remaining periods. 

Since the method finds approximations and, depending on the amount of iterations we make, we're not always guaranteed to find the optimal policy, we will define $N$, the **maximum amount of iterations**, as well as $\varepsilon$, the **tolerated [[Absolute Error|error]]**.

## $n=1$

For the first iteration $n=1$, we will **determine**, for every state $i = 0, 1, \dots, m$:

$$V_{i}^{1} = \mathrm{optimal}\{ C_{ik} \}$$

…having an element to compare for every decision $k$ that is viable in $i$. 

We will then obtain the optimal policy $r_{1}$ (when having $n=1$ remaining periods) by setting $d_{i}\{ r_{1} \}$ to the $k$ that corresponds to the optimal cost. 

We **continue** by setting $n \leftarrow n+1$.

## $n>1$

For the second iteration $n=2$ and onwards, we will **determine**, for every state $i = 0, 1, \dots, m$:

$$
V_{i}^{n} = \mathrm{optimal} \left\{ C_{ik} + \alpha \sum_{j=0}^{m} p_{ij} \{k\}\ V_{j}^{n-1} \right\} 
$$

…having an element to compare for every decision $k$ that is viable in $i$.

We will then obtain the optimal policy $r_{n}$ by setting $d_{i}\{ r_{n} \}$ to the $k$ that corresponds to the optimal cost.

## Stopping Condition

If $n = N$, then we stop iterating. If $n < N$, then, for every state $i = 0, 1, \dots, m$, we test the inequality:

$$
\left| V_{i}^{n} - V_{i}^{n-1} \right| < \varepsilon
$$

If the inequality is satisfied for every $i$, we stop iterating. Otherwise, we set $n \leftarrow n+1$ and continue iterating. 
