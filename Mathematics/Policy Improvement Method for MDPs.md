---
date: 2024-05-18
type: 🧠
tags:
  - MAC/6/PE
---

**Topics:** [[Markov Decision Process]] 

---

The **policy improvement method** can be used to find the optimal [[Policy Improvement Method for MDPs|policy]] for a given [[Markov Decision Process|MDP]].

This method works by, given a policy, relating the [[Expected Total Cost of an MDP Starting from a State|expected total costs starting from a state]] ($V_{i}\{r\}$) with the [[Expected Long Term Cost for a Policy in an MDP|expected long term cost for the policy]] ($g\{r_{n}\}$).

There is a [[Discounted Policy Improvement Method for MDPs|slightly different version of this method that takes into consideration a discount factor]].

# Algorithm

This method is an iterative algorithm. We will use $n$ as the iteration number.

## Step 0

Before we can formally begin, we need to arbitrarily choose a viable policy $r_{1}$ as our starting policy ($n = 1$, first iteration).

## Step 1

The first step is to **solve the following linear equation system**:

$$
\begin{cases}
g\{r_{n}\} &= C_{ik} + \sum_{j=0}^{m} p_{ij}\{k\}\ V_{j}\{r_{n}\} - V_{i}\{r_{n}\} & \text{ for i = 0, 1, ..., m} \\
V_{m} \{r_{n}\} &= 0 &
\end{cases}
$$

…where $C_{ik}$ is the cost of making the decision $k$ in the state $i$ (as defined by the policy) and $p_{ij}\{k\}$ the [[Transition Matrix|transition probability]] from $i$ to $j$ when making the decision $k$ (as defined by the policy). 

We'll thus obtain:

- $g\{r_{n}\}$, the expected long term cost for the policy $r_{n}$
- Every $V_{i}\{r_{n}\}$, the expected total cost starting from a state $i$ given the policy $r_{n}$
	- …where $V_{m}\{r_{n}\}$, the expected total cost starting from the last state in the [[State Set|list of states]], is set to be $0$.

## Step 2

The second step consists in **finding an alternative policy $r_{n+1}$** such that, in every state $i$, $d_{i}\{r_{n+1}\} = k$ is the optimal decision to make. To do so, we will use the values previously we previously obtained (more specifically, every $V_{i} \{ r_{n} \}$).

That is, **for every state $i$**, we will plug these values into the expressions:

$$
C_{ik} + \sum_{j=0}^{m} p_{ij}\{k\}\ V_{j}\{r_{n}\} - V_{i}\{r_{n}\} \quad \text{for k = 1, 2, ..., K} 
$$

…having **one for every decision** that can be made in $i$. We will then pick the decision that yields the optimal result (the smallest if we deal with true costs, the largest if we deal with earnings). This will result in a new alternative policy $r_{n+1}$.

## Step 3

The third and last step is to **determine whether we've obtained the optimal policy** or not, continuing with another iteration if it is not the case.

If $r_{n+1} = r$, then we have the optimal policy. If not, then we shall make another iteration ($n \leftarrow n+1$ and back to step 1). 
