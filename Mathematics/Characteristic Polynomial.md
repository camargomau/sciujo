---
date: 4-20
type: 🧠
tags:
  - MAC/2/ÁL
---

_**Topics**_: [[Algebra]] - [[Eigenvalues and Eigenvectors]]

_**(definition)**_

Let $A \in M_{n \times n} (\mathbb{K})$.

The polynomial $\det(A - \lambda I) = 0$ is called the eigenpolynomial (_polinomio característico_).

_**(definition)**_

Let $T : V \rightarrow V$ and let $\beta$ be a [[basis]] for $V$. We define the eigenpolynomial $f(\lambda)$ of T as:

$$
f(\lambda) = \det(A - \lambda I) = 0
$$

…where $A = [T]_\beta$. It's common to find $\lambda$ denoted as $t$ in books and other documentation.

We solve this polynomial [[Calculation of Eigenvalues and Eigenvectors|find the eigenvalues]] of a given linear transformation.

_**(note)**_

The eigenpolynomial is a polynomial with $n$ degree that has $(-1)^n$ as its [[main coefficient]].

_**(theorem)**_

Let $A \in M_{n \times n} (\mathbb{K})$ and $T : V \rightarrow V$ with $V$ a [[Vector Space|vector space]] with finite [[dimension]].

1. The scalar $\lambda$ is an [[Eigenvalues and Eigenvectors|eigenvalue]] of $A$ $\iff$:
	- $f(\lambda) = \det(A - \lambda I) = 0$
	- $f(\lambda) = \det([T]_\beta - \lambda I) = 0$ ($\beta$ a basis for $V$)
2. $A$ has, at most, $n$ distinct eigenvalues; $T$ has, at most, $n$ distinct eigenvalues

# Equivalences

Let $T : V \to V$ with $V$ a [[Vector Space|vector space]] with $n$ finite [[dimension]].

Let's suppose that the characteristic polynomial of $T$ can be broken down into a product of degree 1 factors. Let $\lambda_1, \dots, \lambda_k$ be _distinct_ eigenvalues of $T$.

Then, the following propositions are [[Equivalence|equivalent]]:

1. $T$ is [[Diagonalisation of a Linear Transformation|diagonalisable]]
2. $V = E_{\lambda_1} \oplus E_{\lambda_2} \oplus \dots \oplus E_{\lambda_k}$
3. If $d_j = \dim(E_j)$ with $1 \leq j \leq k$, then $d_1 + \dots + d_k = n$
4. If $m_j$ is the multiplicity of $\lambda_j$, then $\dim(E_{\lambda_j}) = m_j$
