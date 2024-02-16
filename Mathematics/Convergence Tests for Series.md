---
date: 2022-05-02
type: 🧠
tags:
  - MAC/S2/C2
---

**Topics:** [[Calculus]] - [[Sequence]] - [[Series]]

---

The convergence of [[Series|series]] can be tested with the following tests:

# Sequence Converging to 0

_**(theorem, condición del resto)**_

Let $\sum_{n=1}^{\infty} a_n$ be a [[Limit of a Sequence|convergent sequence]], then:

$$
\lim_{x \to \infty} a_n = 0
$$

This tells us that if the _sequence_ that corresponds to a series doesn't converge to $0$, then the series diverges.

# Comparison Test

_**(theorem)**_

Suppose that $0 < a_n < b_n$ $\forall\ n \in \mathbb{N}$, and that $\sum_{n = 1}^{\infty} b_n$ converges.

Then, $\sum_{n=1}^{\infty} a_n$ converges, and $\sum_{n=1}^{\infty} a_n < \sum_{n=1}^{\infty} b_n$.

# Comparison Test 2

_**(theorem)**_

Let $\sum_{n=1}^\infty a_k$ and $\sum_{n=1}^\infty b_k$ be series, and $a_n, b_n > 0$ $\forall\ n \in \mathbb{N}$. Furthermore, $\lim_{n \to \infty} \frac{a_n}{b_n} = c \neq 0$.

Then $\sum_{n=1}^\infty a_n$ converges if and only if $\sum_{n=1}^\infty b_n$ converges.

# Ratio Test

_**(theorem)**_

Let $a_n > 0$ $\forall\ n \in \mathbb{N}$ and $\lim_{n \to \infty} \frac{a_{n+1}}{a_n} = r$.

Then, $\sum_{n=1}^\infty a_n$ converges if $r<1$ and diverges if $r>1$.

# Integral Test

_**(theorem)**_

Let $\{ a_n \}_{n \in \mathbb{N}}$ be a [[Sequence|sequence]] and $f : \mathbb{R} \to \mathbb{R}$ a non-negative decreasing function, such that $f(n) = a_n$ $\forall\ n \in \mathbb{N}$.

Then, $\int_1^\infty f dx$ (an [[Improper Integral|improper integral]]) converges if and only if $\sum_{n=1}^\infty a_n$ converges.
