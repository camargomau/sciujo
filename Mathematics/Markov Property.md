---
date: 2024-04-04
type: 🧠
tags:
  - MAC/6/PE
---

**Topics:** [[Markov Process]] - [[Stochastic Process]]

---

_**(definition)**_

A [[Stochastic Process|stochastic process]] has the **Markov property** if the probability of future states depends _only_ upon the _present_ state and _not_ the other _past_ states.

Any such stochastic process is also known as a [[Markov Process|Markov process]]. This property is called after the Russian mathematician [[Andrey Markov]]. 

# Formal Definition

_**(definition)**_

More formally, given $\left\{ X_{t} \mid t \in \mathbb{R} \right\}$ a stochastic process, we say it satisfies the **Markov property** if, for any $t$:

$$
\begin{align*}
\mathbb{P}&(X_{t+1} = x_{t+1} \mid X_{0}=x_{0}, \dots ,X_{t-1}=x_{t-1},X_{t}=x_{t}) \\[0.5em]
&= \mathbb{P}(X_{{t+1}} = x_{t+1} \mid X_{t} = x_{t})
\end{align*}
$$

That is, it satisfies the Markov property if the conditional probability of any future result given the present result and every other past result is equal to the conditional probability of any future result given only the present result. 
