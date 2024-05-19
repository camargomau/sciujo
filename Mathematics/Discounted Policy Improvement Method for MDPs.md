---
date: 2024-05-18
type: 🧠
tags:
  - MAC/6/PE
---

**Topics:** [[Policy Improvement Method for MDPs]] - [[Markov Decision Process]]

---

The [[Policy Improvement Method for MDPs|policy improvement method]] can be used to find the optimal [[Policy Improvement Method for MDPs|policy]] for a given [[Markov Decision Process|MDP]]. 

When modelling certain phenomena under certain circumstances, it may prove useful to take a **discount factor** into consideration when determining the optimal policy. Say, for instance, we want to take into consideration the [[Devaluation|devaluation]] of a [[Currency|currency]]. 

For these cases, we can follow a procedure that is practically identical to the one for the policy improvement method, with just a few slight changes in the equations and expressions that are used. The resulting method is called the **discounted policy improvement method**. 

Compared to the standard one, this method only uses the [[Expected Total Cost of an MDP Starting from a State|expected total costs starting from a state]] ($V_{i} \{r\}$), though this time they are actually a variation thereof, since they are discounted. 

> [!info]- Changes Compared to the Standard Method
> The changes in the equations and expressions used for this discounted method compared to the standard one can be summarised as follows:
> - We don't have a $g\{r_{n}\}$ ([[Expected Long Term Cost for a Policy in an MDP|expected long term cost of the policy]])
> - We solve for every $V_{j}\{r_{n}\}$ instead, not setting the last one to $0$
> - We multiply the weighted sum of all the $V_{j}\{r_{n}\}$ by $\alpha$
> - The expressions on the right hand side don't subtract $V_{i}\{r_{n}\}$
> 
> For completeness's sake, and so that this note can stand on its own, I have rewritten all of the steps. 

# Algorithm

This method is an iterative algorithm. We will use $n$ as the iteration number.

## Step 0

Before we can formally begin, we need to arbitrarily choose a viable policy $r_{1}$ as our starting policy ($n = 1$, first iteration).

Of course, we also have to define a **discount factor** $\alpha$. We can alternatively define an **interest rate** $i$, having:

$$
\alpha = \frac{1}{1+i} = (1+i)^{-1}
$$

## Step 1

The first step is to **solve the following linear equation system**:

$$
\begin{cases}
V_{i}\{r_{n}\} &= C_{ik} + \alpha \sum_{j=0}^{m} p_{ij}\{k\}\ V_{j}\{r_{n}\} & \text{ for i = 0, 1, ..., m}
\end{cases}
$$

…where $C_{ik}$ is the cost of making the decision $k$ in the state $i$ (as defined by the policy) and $p_{ij}\{k\}$ the [[Transition Matrix|transition probability]] from $i$ to $j$ when making the decision $k$ (as defined by the policy). 

We'll thus obtain every $V_{i}\{r_{n}\}$, the expected total cost starting from a state $i$ given the policy $r_{n}$.

## Step 2

The second step consists in **finding an alternative policy $r_{n+1}$** such that, in every state $i$, $d_{i}\{r_{n+1}\} = k$ is the optimal decision to make. To do so, we will use the values previously we previously obtained.

That is, **for every state $i$**, we will plug these values into the expressions:

$$
C_{ik} + \alpha \sum_{j=0}^{m} p_{ij}\{k\}\ V_{j}\{r_{n}\} \quad \text{for k = 1, 2, ..., K} 
$$

…having **one for every decision** that can be made in $i$. We will then pick the decision that yields the optimal result (the smallest if we deal with true costs, the largest if we deal with earnings). This will result in a new alternative policy $r_{n+1}$.

## Step 3

The third and last step is to **determine whether we've obtained the optimal policy** or not, continuing with another iteration if it is not the case.

If $r_{n+1} = r$, then we have the optimal policy. If not, then we shall make another iteration ($n \to n+1$ and back to step 1). 
