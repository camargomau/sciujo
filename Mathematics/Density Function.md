---
date: 2023-03-06
type: 🧠
tags:
  - MAC/4/PB
  - MAC/5/E1
---

**Topics:** [[Probability]] - [[Random Variable]]

---

_**(definition)**_

Let $X$ be a real [[Random Variable|random variable]] whose [[Range of a Function|range]] is $R_X$.

A density function is a function that allows us to specify the probability of $X$ being a specific value (in the discrete case) or of $X$ falling within a particular range of values (in the continuous case, though indirectly, as you'll see below).

# Discrete Random Variables

When $X$ is a [[Discrete Random Variable|discrete random variable]], we define the _density function_ of $X$ as the [[Function|function]] $f_X : R_X \subset \mathbb{R} \to [0, 1]$ as:

$$
f_X(x) =
\begin{cases}
\mathbb{P}(X = x) & \text{if } x \in R_X \\
0 & \text{otherwise}
\end{cases}
$$

 …and the following must hold:

1. $$0 \leq f_X(x) \leq 1$$
2. $$\sum_{x \in R_X} f_X(x) = 1$$

The density function of a _discrete_ random variable does tell us the probability that the random variable takes _exactly_ a _specific_ value.

The density function of a discrete random variable is also called a _mass function_.

# Absolutely Continuous Random Variables

> [!info]- Continuous vs. Discrete Density Functions
> Notice that, when the random variable $X$ takes discrete values, we can find the probability that $X$ is _exactly_ a _specific_ value, hence why we defined it the way we did.
>
> We can't do the same with absolutely continuous random variables, since there is an infinite amount of possible values in any given interval. The probability of $X$ being _exactly_ a _specific_ value is $0$.
>
> Instead, we will define the density function to be an integrable function whose _integral_ over a given interval gives us the probability that the random variable falls _within_ that interval.
>
> Basically: for absolutely continuous random variables, the density function does **not** define the probabilities; rather, it is the area under its curve (its **integral**) that does.
>
> It does **not** tell us the probability of $X$ being a _specific_ value, it simply tells us, by means of its integral, the probability of $X$ being in _range_ of values.
>
> Indeed, its integral is basically the random variable's [[Distribution Function|distribution function]].

When $X$ is an [[Absolutely Continuous Random Variable|absolutely continuous random variable]], we define the _density function_ of $X$ as the [[Function|function]] $f_X : R_X \subset \mathbb{R} \to \mathbb{R}_+ = [0, \infty)$ as:

$$
f_X(x) = \begin{cases}
\text{a function} & \text{if } x \in \text{relevant interval} \\
0 & \text{otherwise}
\end{cases}
$$

 …and the following must hold:

1. $$f_X \geq 0$$

2. $$\int_{\mathbb{R}} f_X(x)\ dx = 1$$

Many times, when simply saying _density function_, an absolutely continuous random variable is implied (with the discrete case using _mass function_).
