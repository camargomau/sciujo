---
date: 2024-02-07
type: 🧠
tags:
  - MAC/6/PE
---

**Topics:** [[Stochastic Process]]

---

Empirically, we have a **stochastic process** whenever we're studying the behaviour of a [[Random Variable|random variable]] across time. We'll be working with stochastic processes when trying to model the future behaviour of a given process. 

# (Almost Formal) Definition

_**(definition)**_

A **stochastic process** is a [[Sequence|sequence]] of random variables $\left\{X_{n} \mid n \in \mathbb{N}\right\}$, where the sub-index indicates the corresponding time or space. 

This idea can be generalised so that the time instants are continuous; that is, $\left\{X_{t} \mid t \in \mathbb{R}\right\}$.

# (Formal) Definition

_**(definition)**_

Given the [[Probability Space|probability space]] $(\Omega, \alpha, \mathbb{P})$ such that for every fixed $t \in T \subset \mathbb{R}$, we have:

$$
X_{t} : (\Omega, \alpha, \mathbb{P}) \to X_{t}(\omega) \in \mathbb{R}
$$

That is, $X_{t}$ is a [[Random Variable|random variable]] and for every fixed $\omega \in \Omega$, $X_{t}(\omega)$ is a time [[Function|function]].

Generally, we'll think of the sub-index $t$ as the time indicator and of $X_{t}$ as the state/position of the stochastic process at the instant $t$.

