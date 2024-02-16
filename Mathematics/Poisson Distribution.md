---
date: 2023-04-24
type: 🧠
tags:
  - MAC/S4/PB
---

**Topics:** [[Probability]]

---

_**(definition)**_

Let $X$ be a [[Discrete Random Variable|discrete random variable ]] that handles the number of events that occur a given time or space interval, knowing that these events occur with a known constant mean rate and [[Event Independence|independently]] of the time since the last event.

For such an $X$, we write:

$$
X \sim \mathrm{Poi}(\lambda)
$$

…where $\lambda$ is the parameter that represents the number of times that an event is expected to occur in a given interval ($\lambda > 0$). We use this interval and its $\lambda$ as our main references when talking about a Poisson distribution.

# Density Function

_**(theorem)**_

With an $X$ such that $X \sim \mathrm{Poi}(\lambda)$, its [[Density Function|density function]] is:

$$
f_{X}(x) =
\begin{cases}
\frac{\lambda^x e^{-\lambda}}{x!} &\text{if } x = 0, 1, \dots, \infty \\
0 &\text{otherwise}
\end{cases}
$$

> [!abstract]- Proof that this is a density function
> Remember that $f_{X}(x)$ is a density function if:
>
> $$
> \sum_{x \in R_{X}} f_{X}(x) = 1
> $$
>
> The density function given here is, effectively, a density function, since:
>
> $$
> \begin{align*}
> \sum_{x=0}^\infty \frac{\lambda^x e^{-\lambda}}{x!} &= e^{-\lambda} \sum_{x=0}^\infty \frac{\lambda^x}{x!} \\
> &= e^{-\lambda} e^\lambda \\
> &= 1
> \end{align*}
> $$

# Expected Value

_**(theorem)**_

Such an $X$ has a very simple [[Expected Value|expected value]]:

$$
\mathbb{E}[X] = \lambda
$$

# Variance

_**(theorem)**_

Such an $X$ also has a very simple [[Variance|variance]]:

$$
\mathrm{Var}(X) = \lambda
$$

Notice it's the same as its expected value.

# Moment-Generating Function

_**(theorem)**_

As for the [[Moment-Generating Function|moment-generating function]] of such an $X$, it is:

$$
M_X(t) = e^{\lambda (e^t - 1)}
$$

# Example

Let $X$ be the number of messages that are rejected by a web server in a second. We know that 5 messages are expected to be rejected every second (i.e. we know that $X \sim \mathrm{Poi}(5)$).

We'll calculate:

1. The probability that exactly 3 messages are rejected in a second
2. The probability that at most 2 messages are rejected in a second.

## Exactly 3 messages

Since $X$ is [[Discrete Random Variable|discrete]], we can simply evaluate the density function at $x = 3$:

$$
\mathbb{P}(X=3) = f_{X}(3) = \frac{5^3 e^{-5}}{3!} \approx 0.1403
$$

## At most 2 messages

From the idea of a [[Distribution Function|distribution function]], we have that:

$$
\begin{align*}
\mathbb{P}(X \leq 2) &= \mathbb{P}(X=0) + \mathbb{P}(X=1) + \mathbb{P}(X=2) \\
&= \frac{5^0 e^{-5}}{0!} + \frac{5^1 e^{-5}}{1!} + \frac{5^2 e^{-5}}{2!} \\
&\approx 0.12465
\end{align*}
$$
