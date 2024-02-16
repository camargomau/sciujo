---
date: 2022-04-18
type: 🧠
tags:
  - MAC/S2/ÁL
aliases:
  - diagonalisable
---

**Topics:** [[Algebra]] - [[Linear Transformation]]

---

_**(definition)**_

We say that $T : V \rightarrow V$, a [[Linear Transformation|linear transformation]], with $V$ a [[Vector Space|vector space]] on $\mathbb{K}$, is _diagonalisable_ if there exists a [[basis]] $\beta$ for $V$ such that $[T]_{\beta}$ is a [[diagonal matrix]].

A matrix $A \in M_{n \times n} (\mathbb{K})$ is diagonalisable if $A$ is [[similar]] to a diagonal matrix. That is, if there exists a $Q$ such that:

$$
A = Q^{-1}\ B\ Q
$$
…where $B$ is a diagonal matrix. $Q$ can be found by means of [[Eigenvalues and Eigenvectors|eigenvalues and eigenvectors]].

# Equivalences

_**(theorem, important)**_

Let $T : V \rightarrow V$ with $V$ a vector space on $\mathbb{K}$ with finite [[dimension]].

Then, the following statements are equivalent:

1. $T$ is diagonalisable
2. There exists a [[basis]] $\beta$ for $V$ such that $[T]_\beta$ is diagonalisable
3. The matrix $[T]_\gamma$ is diagonalisable for any basis $\gamma$ of $V$

_**(corollary)**_

A matrix $A$ is diagonalisable if and only if $L_A$ is diagonalisable.
