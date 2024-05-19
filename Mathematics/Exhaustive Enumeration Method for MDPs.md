---
date: 2024-05-18
type: 🧠
tags:
  - MAC/6/PE
---

**Topics:** [[Markov Decision Process]] - [[Optimisation]]

---

Given an [[Markov Decision Process|MDP]], we can find the optimal [[Markov Decision Process Policy|policy]] with the **exhaustive enumeration method**. This method is one of the simplest for this purpose.

# Algorithm

The exhaustive enumeration method consists of the following steps.

## Step 1

**Enumerating _exhaustively_ all of the _viable_ policies for the MDP.**

- When every decision (with $k$ total) can be made in every [[State Set|state]] (with $m+1$ total), then the total amount of viable policies is $k^{m+1}$ ([[Permutations with Repetitions|permutations with repetitions]]).

## Step 2

**Calculating the [[Expected Value|expected]] _long term_ cost for every policy $r$:**

$$
\mathbb{E}[C_{r}] = \sum_{i=0}^{m} C_{ik} \pi_{i}
$$

…where $C_{ik}$ denotes the cost incurred for making the decision $k$ (defined _according to the policy_) in the state $i$, while $\pi_{i}$ denotes the [[Steady State Probability|steady state probability]] of the state $i$ _given the policy_. 

**Don't forget to take the policy into consideration in this step**. It defines the decision $k$ we'll be taking in each state $i$, as well as the [[Transition Matrix|transition matrix]] that is used to obtain the steady state probabilities. We can obtain the latter by (1) selecting the column that corresponds to the state $i$ in the transition matrix for the decision $k$, and then (2) splicing them together in a new matrix. 

## Step 3

**Select the _optimal_ policy based on its cost.**

If we're dealing with classical costs, then we'll select the policy that has the smallest expected cost. If our "costs" are actually earnings, then we'll select the policy that has the largest expected "cost" (earning). 
