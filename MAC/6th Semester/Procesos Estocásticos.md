---
type: 🏫
tags:
  - MAC/6/PE
---

# Unit 1: Introduction to Stochastic Processes

A [[Stochastic Process|stochastic process]] can be, broadly, analysed as a sequence $\left\{ X_{t} \mid t \in \mathbb{R} \right\}$ of random variables, each of them corresponding to a specific moment in time, place, instance, etc. 

The [[State Set|state set]] of a stochastic process is the set of all possible values that the random variables $X_{t}$ in the process can take. Similarly, the [[Parameter Set|parameter set]] of a stochastic process is the set of all possible values that its parameter $t$ can take. 

## Types of Stochastic Processes

We can classify stochastic processes according to the nature of their state set $S$ and parameter set $T$:

| $S$ / $T$  | Discrete                                                       | Continuous                                 |
| ---------- | -------------------------------------------------------------- | ------------------------------------------ |
| Discrete   | [[Chain]]                                                      | [[Point Process\|Point process]]           |
| Continuous | [[Sequence of Random Variables\|Sequence of random variables]] | [[Continuous Process\|Continuous process]] |

Moreover, we can also classify them according to the probabilistic features of its random variables:

- An [[Independent Trial Process|independent trial process]] is a stochastic process with a discrete parameter set and independent random variables.
- A [[Markov Process|Markov process]] is a stochastic process that satisfies the [[Markov Property|Markov property]].
- A [[Stochastic Process with Independent Increments|process with independent increments]] is a stochastic process whose every increment between any two random variables is independent. 
- A [[Stationary Process|stationary process]] is a stochastic process that has the same probability distribution for the vector of random variables, regardless of the value that its parameter takes.

## Bernoulli Process

A [[Bernoulli Process|Bernoulli process]] is a stochastic process that behaves according to the Bernoulli trial.

Each random variable in it will follow a Bernoulli distribution, while the stochastic process that follows the sum of successes will consist of random variables that follow a binomial distribution.

## Random Walk

A [[Random Walk|random walk]] is a stochastic process whose state set is $\mathbb{Z}$ and parameter set is $\mathbb{N}$, where there's a probability $p$ of moving to the next integer and $q$ of moving to the previous one. 

When a random walk starts at $0$, we say it is a simple random walk.

There are [[Transition Probabilities in a Random Walk|several formulae that can help us calculate the transition probabilities in a random walk]]. 

## Gambler's Ruin Problem

The [[Gambler's Ruin Problem|gambler's ruin problem]] is a random walk that studies a game between two players where they give each other a monetary unit upon loss. 

In the context of this problem, we can obtain the [[Probability of Ruin in the Gambler's Ruin Problem|probability of a given player getting ruined]], as well as the [[Expected Amount of Bets Before Ruin in the Gambler's Ruin Problem|expected amount of bets before a given player gets ruined]].

# Unit 2: Markov Chains

A [[Markov Chain|Markov chain]] is a chain (i.e. a stochastic process with both a discrete state set and a parameter set) that satisfies the [[Markov Property|Markov property]]. 

## Transition Probabilities

In Markov chains, [[Transition Probabilities in a Markov Chain|the study of transition probabilities]] is of special interest. We can define:

- [[One Step Transition Probability|One step transition probabilities]], the probabilities of transitioning from one state to another in a single step. 
- [[Stationary Transition Probability|Stationary transition probabilities]], which show up when the transition probabilities in a Markov chain don't change across time.

The existence of stationary transition probabilities also allow us to define [[n Step Transition Probability|n step transition probabilities]], which prove to be quite useful. Additionally, it can be handy to write these probabilities in a [[Transition Matrix|transition matrix]]. The $n$ step transition matrix can be easily obtained by calculating the $n$th power of the corresponding one step matrix. 

## More on Transition Probabilities

For any type of stochastic process, we can define an [[Initial Probability Vector|initial probability vector]], which contains the probabilities of having each possible state being the initial state in the process. 

A [[Finite and Stationary Markov Chain|finite and stationary Markov chain]] is a Markov chain with a finite state set and stationary transition probabilities. 

The [[Chapman-Kolmogorov Equation|Chapman-Kolmogorov equation]] is an equation that helps us calculate the $n$ step transition probabilities through a sum of products of probabilities. 

The transition probabilities that have been mentioned previously are actually _conditional_ in the sense that they consider a specific present state. We can additionally obtain the [[Unconditional Transition Probability|unconditional transition probabilities]], which are the probabilities of reaching a given state with no other condition specified. 

## Communication and Classes

When it is possible to go from a state $i$ to another $j$, we say that $j$ is accessible from $i$. When that happens and $i$ is also accessible from $j$, we say that [[State Communication|these two states communicate]].

When grouping _all_ states that communicate, we obtain [[Markov Chain State Class|classes]]. 

## Ergodic, Transitory and Absorbing States

An [[Ergodic Set|ergodic set]] is a set of states from which it is no longer possible to get out once reached. A Markov chain with only one class is said to be [[Ergodic Markov Chain|ergodic]].

An [[Absorbing Set|absorbing set]] is an ergodic set that only has _a single_ element. 

A [[Transitory Set|transitory set]] is basically the opposite of an ergodic set: a set from which it is still possible to get out once reached. Since every Markov chain must have at least one ergodic set, then it follows that we may exit a transitory state and never come back to it. 

The states in an ergodic set, absorbing set and transitory set are called ergodic, absorbing and transitory, respectively.

