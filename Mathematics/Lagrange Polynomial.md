---
date: 2023-02-07
type: 🧠
tags:
  - MAC/S4/MN2
---

**Topics:** [[Polynomial]] - [[Numerical Analysis]]

---

Let us have $n+1$ [[Point|points]] $(x_0, y_0), \dots, (x_n, y_n)$, with $x_i \neq x_j$ when $i \neq j$ (i.e. all abscissas distinct).

We will build a polynomial of degree $n$, called the _Lagrange (interpolation) polynomial_, that will allow us to [[Interpolation|interpolate]] this sequence of points.

# Lagrange Basis

_**(definition)**_

We define the _Lagrange [[Basis|basis]]_ as the [[Set|set]] of [[Polynomial|polynomials]] $\{ l_0(X), l_1(X), \dots, l_n(X) \}$, where:

$$
\begin{align}
l_i(X)  &= \prod_{\substack{j=0 \\ j \neq i}}^n \frac{X-x_j}{x_i-x_j} \\
&= \left( \frac{X - x_0}{x_i - x_0} \right) \dots \left( \frac{X - x_{i-1}}{x_i - x_{i-1}} \right) \left( \frac{X - x_{i+1}}{x_i - x_{i+1}} \right) \dots \left( \frac{X - x_n}{x_i - x_n} \right)
\end{align}
$$

In particular, notice that:

1. $l_i(X)$ is of [[Degree of a Polynomial|degree]] $n$ for all $i$
2. $\mathcal{l}_i = \begin{cases} 0 \text{ if } X \neq x_i \\ 1 \text{ if } X = x_i \end{cases}$

(see [[Kronecker Delta|Kronecker delta]])

# Lagrange Polynomial

_**(definition)**_

We define the _Lagrange (interpolation) polynomial_ as the linear combination:

$$
\begin{align}
L(X) &= \sum_{j=0}^n l_j(X)\ y_j \\
&= l_0(X)\ y_0 + l_1(X)\ y_1 + \dots + l_n(X)\ y_n
\end{align}
$$

This polynomial is special in that for all $i$, $L(x_i) = y_i$. This happens thanks to the Kronecker delta-like behaviour of the polynomials in the basis.

This allows us to use the polynomial to [[Interpolation|interpolate]] the initial sequence of points.
