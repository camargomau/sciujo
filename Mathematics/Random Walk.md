---
date: 2024-02-18
type: 🧠
tags:
  - MAC/6/PE
---

**Topics:** [[Stochastic Process]]

---

_**(definition)**_

Let $\left\{ X_{n} \mid n \in \mathbb{N} \right\}$ be a [[Stochastic Process|stochastic process]] with $S = \mathbb{Z}$ as its [[State Set|state set]]. Note that it has a discrete [[Parameter Set|parameter set]] $\mathbb{N} = \{ 0, 1, 2, \dots \}$. 

Let $X_{0} = a$ and let, for any $n \in \mathbb{N}$:

$$
\mathbb{P}\left( X_{n+1} = j \mid X_{n} = i \right)
=
\begin{cases}
p & \text{if } j = i + 1 \\
q & \text{if } j = i - 1 \\
0 & \text{otherwise}
\end{cases}
$$

We call such a stochastic process a **random walk**. When $X_{0} = a = 0$, we call it a **simple** random walk.

Do note that these probabilities don't depend on the specific $k$ and, as such, we say that they are _homogeneous across time_. A simple random walk is a [[Markov Process|Markov process]].

[[Transition Probabilities in a Random Walk|We can deduce several formulae]] that make it easier to obtain the [[Transition Probability|transition probabilities]] in a random walk.

# Formal Definition

_**(definition)**_

Let $\varepsilon_{1}, \varepsilon_{2}, \dots$ be a sequence of [[Independent and Identically Distributed Random Variables|iid random variables]] such that, for any $k$:

- $\mathbb{P}(\varepsilon_{k} = 1) = p$ 
- $\mathbb{P}(\varepsilon_{k} = -1) = q$

…where $p + q = 1$.

With that, we define a **random walk** as the stochastic process $\left\{ X_{n} \mid n \in \mathbb{N} \right\}$ where $X_{0} = a$ and, for $n \geq 1$:

$$
X_{n} = X_{0} + \varepsilon_{1} + \varepsilon_{2} + \dots + n
$$

Recall that when $X_{0} = a = 0$, we call it a **simple** random walk.

# Symmetrical and Asymmetrical Walks

_**(definition)**_

Recall that $p+q=1$. When $p = q = \frac{1}{2}$, we say that the random walk is symmetrical. When $p \neq q$, we say it is asymmetrical.

# Expected Value and Variance

_**(theorem)**_

For any integer $n \geq 0$, we have:

$$
\begin{align*}
\mathbb{E}[X_{n}] &= n(p-q) \\
\mathrm{Var}(X_{n}) &= 4npq
\end{align*}
$$
