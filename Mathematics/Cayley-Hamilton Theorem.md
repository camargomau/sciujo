---
date: 2022-05-04
type: 🧠
tags:
  - MAC/2/ÁL
---

**Topics:** [[Algebra]] - [[Diagonalisation of a Linear Transformation]]

---

This theorem assures us that $T : V \to V$ a [[Linear Transformation|linear transformation]] (with $V$ a [[Vector Space|vector space]] on $\mathbb{K}$ with finite [[dimension]]) nullifies its own [[Characteristic Polynomial|characteristic polynomial]].

_**(theorem)**_

Let $T : V \to V$ be a [[Linear Transformation|linear transformation]], and $f(t)$ be its characteristic polynomial.

Then, $f(T) = T_0$

_**(corollary)**_

Let $A \in M_{n \times n} (\mathbb{K})$ be the [[Associated Matrix of a Linear Transformation|associated matrix]] of $T$, and $f(t)$ be its characteristic polynomial.

Then, $f(A) = 0$.

# Theorem applications

## Finding the inverse of $A$

We'll find the inverse of $A = \begin{pmatrix} 1 & 2 \\ 2 & 1 \end{pmatrix}$.

### 1. Find the characteristic polynomial

$$
f(\lambda) = \det \begin{pmatrix} 1 - \lambda & 2 \\ 2 & 1 - \lambda \end{pmatrix} = \lambda^2 - 2\lambda - 3
$$

We then substitute $\lambda$ for $A$, and multiply the constant term by the identity matrix:

$$
A^2 - 2A - 3I = 0
$$

(it's equal to $0$ since the theorem tells us that the characteristic polynomial is nullified).

Continuing:

$$
A^2 - 2A = 3I
$$

$$
A(A - 2I) = 3I
$$

We then multiply this by $A^{-1}$:

$$
A^{-1} A (A-2I) = 3A^{-1} I = 3A^{-1}
$$

$$
A-2I = 3A^{-1}
$$

$$
\frac{A-2I}{3} = A^{-1}
$$

Operating with the actual matrix, we get:

$$
\frac{1}{3} \begin{pmatrix} -1 & 2 \\ 2 & -1 \end{pmatrix} = \begin{pmatrix} -\frac{1}{3} & \frac{2}{3} \\ \frac{2}{3} & -\frac{1}{3} \end{pmatrix}
$$

Voilà. We got that $A^{-1} = \begin{pmatrix} -\frac{1}{3} & \frac{2}{3} \\ \frac{2}{3} & -\frac{1}{3} \end{pmatrix}$.
