---
date: 2023-03-06
type: 🧠
tags:
  - MAC/S4/PB
  - MAC/S5/E1
aliases:
  - random variable
---

**Topics:** [[Probability]]

---

_**(definition)**_

A _random variable_ $X$ is a [[Measurable Function|measurable function]] $X : \Omega \to \mathbb{R}$ ($\Omega$ a [[Sample Space|sample space]]) where, given any [[Set|set]] $B$:

$$
X^{-1}(B) \in \mathscr{F}
$$

…or also:

$$
\left\{ w \in \Omega \mid X(w) \leq x \right\} \in \mathscr{F}
$$

…where $\mathscr{F}$ is a [[σ-Algebra|sigma-algebra]].

In other words, a random variable is a mapping from the possible outcomes in the sample space to a measurable space (in this case $\mathbb{R}$).

As such, in general, we can see a random variable as the mathematical formalisation of quantities or objects that depend on randomness.

> [!info]- Notation
> Uppercase letters, like $X, Y, Z$, denote the random variable itself. On the other hand, lowercase letters, like $x, y, z$, denote a value that the corresponding random variable may take.
>
> With this, we can write the [[Range|range]] of a random variable $X$ as:
>
> $$
> R_X = \{ x_1, x_2, x_3, \dots \}
> $$

# Types

There are two types of random variables:

- [[Discrete Random Variable|Discrete random variables]]
- [[Absolutely Continuous Random Variable|Absolutely continuous random variables]]

For both of these, we can define a [[Density Function|density function]], which helps us specify the probability of the random variable being a certain value or being in a given interval.
