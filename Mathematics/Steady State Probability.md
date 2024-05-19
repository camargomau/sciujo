---
date: 2024-04-04
type: 🧠
tags:
  - MAC/6/PE
---

**Topics:** [[Regular Markov Chain]] - [[Markov Chain]]

---

In a regular Markov chain, it happens that, regardless of the initial state, the probability of reaching a given state is a _constant_ when the number of steps is sufficiently high. 

_**(fundamental theorem)**_

For every regular Markov chain, the following limit ([[n Step Transition Probability|n step transition probability]]) exists and it's the same one regardless of $i$:

$$
\pi_{j} = \lim_{ n \to \infty } p_{ij}^{(n)}
$$

Furthermore, we have that $\pi_{j} \geq 0$ and the following equations are satisfied:

1. $\pi_{j} = \sum_{i=0}^{m} \pi_{i} p_{ij}$, for $j = 0, 1, 2, \dots, m$
2. $\sum_{j=0}^{m} \pi_{j} = 1$

The values $\pi_{j}$ are called **steady state probabilities**, while the vector that they form is called the **stationary distribution vector**. 

In other words, the probability of reaching a state $j$ tends to $\pi_{j}$ as $n \to \infty$, regardless of the initial state. 

# Calculation of Steady State Probabilities

_**(observation)**_

We can calculate all of the $\pi_{j}$ in a given chain by formulating all corresponding equations then solving the resulting equation system. 

Notice that this resulting equation system has $m+2$ equations _but_ only $m+1$ unknowns. This system has a unique solution, so one of these equations will be redundant. 

Thus, we may find it easier to solve the system that consists of all equations _but one_ (the redundant one). Note that the equation that establishes that all $\pi_{j}$ must add up to $1$ is never redundant, so it can never be discarded. 

# Transitory States Tend to 0

_**(corollary)**_

If $j$ is a [[Transitory Set|transitory state]], then:

$$
\lim_{ n \to \infty } p_{ij}^{(n)} = \pi_{j} = 0
$$

…since, the more steps we take, the more likely we are to step out of its containing (transitory) set and thus, stop being able to return to it. 

# Limit of the Transition Matrix

_**(corollary)**_

From the previous theorem, it's also possible to observe that, given $P^{(n)}$ the [[Transition Matrix|n step transition matrix]] of the regular Markov chain:

$$
\lim_{ n \to \infty } P^{(n)} =
\begin{pmatrix}
\pi_{0} & \pi_{1} & \dots & \pi_{m} \\
\pi_{0} & \pi_{1} & \dots & \pi_{m} \\
\vdots & \vdots & \ddots & \vdots \\
\pi_{0} & \pi_{1} & \dots & \pi_{m} \\
\end{pmatrix}
$$

