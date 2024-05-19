---
date: 2024-05-18
type: 🧠
tags:
  - MAC/6/PE
aliases:
  - "MDP"
---

**Topics:** [[Markov Chain]] - [[Stochastic Process]]

---

_**(definition)**_

A **Markov decision process** (MDP) is a [[Markov Chain|Markov chain]] characterised by the ability to make a decision (among various options) in each state, incurring a cost for each decision taken in a given state. 

MDPs can model diverse phenomena, making them useful when paired with [[Optimisation|operations research/optimisation]]. In this regard, [[Optimisation Methods for Markov Decision Processes|several methods]] allow us to find the optimal [[Markov Decision Process Policy|policy]] for a given MDP. 

# Characterisation

An MDP is characterised by the following 4 elements:

- $S = \{ 0, 1, 2, \dots, m \}$, its [[State Set|state set]]
- $K = \{ 1, 2, \dots, k \}$, its set of decisions
- $C_{ik}$, the costs associated to taking the decision $k$ in the state $i$
- The [[Transition Matrix|transition matrices]] associated to a given decision $k$, whose elements are commonly denoted by $p_{ij}\{k\}$

Additionally, we may define $R = \left( r_{1}, r_{2}, \dots \right)$, the set of [[Markov Decision Process Policy|policies]] that can be formed with all the viable decisions in each state.
