---
date: 2024-05-18
type: 🧠
tags:
  - MAC/6/PE
---

**Topics:** [[Markov Decision Process]] - [[Linear Programming Problem]]

---

Given an [[Markov Decision Process|MDP]], we can find the optimal [[Markov Decision Process Policy|policy]] by formulating it as a [[Linear Programming Problem|linear programming problem]]. 

# Decision Variables

## As Binary

Let the following be our decision variables:

$$
D_{ik} =
\begin{cases}
1 & \text{if the decision } k \text{ is made in the state } i \\
0 & \text{otherwise}
\end{cases}
$$

Once solved, the matrix of the values these variables optimally take characterises the optimal policy. 

## As Continuous

Solving binary linear programming problems isn't as straightforward as it may normally be with continuous ones, so we can reinterpret these decision variables as:

$$
D_{ik} = \mathbb{P}(k \mid i)
$$

Id est, the probability of making the decision $k$ given that the state is in the [[State Set|state set]] $i$. 

Under this reinterpretation, we'll be actually using other variables in the [[Objective Function|objective function]]: $Y_{ik}$. These represent the [[Unconditional Transition Probability|unconditional]] [[Steady State Probability|steady state probability]] of being in the state $i$ _and_ taking the decision $k$, satisfying:

$$
D_{ik} = \frac{Y_{ik}}{\sum_{k=1}^{K} Y_{ik}}
$$

# Model

Finally, with these considerations, the linear programming model for an MDP is:

$$
\begin{cases}
&\text{optimise } \mathbb{E}[C] = Z = \sum_{i=0}^{m} \sum_{k=1}^{K} C_{ik} Y_{ik} & \\[1em]
& \text{s.t.} & \\[0.5em]
&\sum_{i=0}^{m} \sum_{k=1}^{k} Y_{ik} = 1 \\[0.5em]
&\sum_{k=1}^{K} Y_{jk} - \sum_{i=0}^{m} \sum_{k=1}^{K} Y_{ik}\ p_{ij} \{k\} = 0 \quad \text{for } j = 0, 1, \dots m
\end{cases}
$$

…where:

- $C_{ik}$ denotes the cost of making the decision $k$ in the state $i$
- $p_{ij}\{k\}$ denotes the [[Transition Matrix|transition probability]] from state $i$ to $j$ when making the decision $k$

Evidently, we can find the optimal $Y_{ik}$ by solving this linear programming problem through any of the applicable methods ([[Simplex Method|simplex]], etc.). Then we can determine the optimal policy by calculating the $D_{ik}$ as established above.
