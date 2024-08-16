---
date: 2022-08-16
type: 🧠
tags:
  - MAC/3/MN1
aliases:
  - normalised
  - normalised form
  - Normalised
  - Normalised Form
---

**Topics:** [[Numerical Analysis]] - [[Rounding Error]]

---

To represent [[Real Numbers|real numbers]] on a computer, the first step is to first obtain its _normalised form_:

$$
\pm 0.d_1d_2d_3\dots d_k \times B^e
$$

…where:

- $d_1$: a digit with a value from $1$ to $(B-1)$
- $d_i$: digits with values from $0$ to $(B-1)$
- $B$: numerical base ($2, 8, 16, 10$)
- $k$: number of significative digits ([[Precision|precision]])
- $e$: exponent (an [[Integers|integer]])

These normalised numbers can then be used to obtain their [[Floating Point Form of Real Numbers|floating point form]].

The representation of $0$ is special.

> [!example]- Examples
> | **Number**    | **Normalised form**            |
> | ------------- | ------------------------------ |
> | $15.812$      | $+0.15812 \times 10^2$         |
> | $-0.0527$     | $-0.527 \times 10^{-1}$        |
> | $0.00325$     | $+0.325 \times 10^{-2}$        |
> | $15635.00236$ | $+0.1563500236 \times 10^{-5}$ |
