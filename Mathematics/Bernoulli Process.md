---
date: 2024-02-16
type: 🧠
tags:
  - MAC/6/PE
---

**Topics:** [[Stochastic Process ]]- [[Bernoulli Trial]]

---

_**(definition)**_

A [[Stochastic Process|stochastic process]] $\left\{ X_{n} \mid n \in \mathbb{N} \right\}$ is called a **Bernoulli process** if it satisfies the following conditions:

1. $X_{1}, X_{2}, \dots$ are [[Event Independence|independent]]
2. $\mathbb{P}(X_{n} = 1) = p$, $\mathbb{P}(X_{n} = 0) = 1-p = q$

We'll refer to the event $X_{n} = 1$ as _success_ and to $X_{n} = 0$ as _failure_.

# Number of Successes

_**(definition)**_

Let $\left\{ X_{n} \mid n \in \mathbb{N} \right\}$ be a Bernoulli process with a success probability of $p$. 

The number of successes we've had up to the $n$th trial is denoted by $N_{n}$ and defined as:

$$
N_{n} =
\begin{cases}
0 & \text{if } n = 0 \\
X_{1} + \dots + X_{n} & \text{if } n = 1, 2, 3, \dots \\
\end{cases}
$$

Note that $N_{n}$ defines another stochastic process, one with discrete [[State Set|state]] and [[Parameter Set|parameter]] sets.

_**(observation)**_

From the previous definition, we can tell that $N_{n+m} - N_{n}$ is the number of successes we've had along the trials $n+1, n+2, \dots, n+m$.

# Distribution of $X_{n}$ and $N_{n}$

_**(theorem)**_

Each of these individual $X_{n}$ follow a [[Bernoulli Distribution|Bernoulli distribution]] with a parameter $p$. 

As such, $N_{n}$ follows a [[Binomial Distribution|binomial distribution]] with parameters $n,p$, since the sum of independent Bernoulli-distributed [[Random Variable|random variables]] distributes binomially. 

_**(theorem)**_

Now, we can tell that for $n \in \mathbb{N}$:

1. $\mathbb{P}(N_{n} = k) = \binom{n}{k} p^{k} q^{n-k} \qquad k = 0, 1, \dots, n$
2. $\mathbb{E}[N_{n}] = np$
3. $\mathrm{Var}(N_{n}) = npq$

Basically what was already established for a [[Bernoulli Distribution|Bernoulli distribution]].
