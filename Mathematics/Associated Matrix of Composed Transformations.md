---
date: 2022-04-01
type: 🧠
tags:
  - MAC/2/ÁL
---

**Topics:** [[Algebra]] - [[Linear Transformation]]

---

_(theorem)_

Let $U, V, W$ be [[Vector Space|vector spaces]] on $\mathbb{K}$ where $\dim(V) = s$, $\dim(V) = n$, $\dim(W) = t$.

Let:

- $\beta = \{ u_1, \dots, u_s \}$ be a [[basis]] of $U$
- $\gamma = \{ v_1, \dots, v_n \}$ be a basis of $V$
- $\delta = \{ w_1, \dots, w_t \}$ be a basis of $W$

…and let $S : U \rightarrow V$ and $T : V \rightarrow W$ be [[Linear Transformation|linear transformations]].

Then, the [[Associated Matrix of a Linear Transformation|associated matrix]] of $T \circ S$ ([[Linear Transformation Composition|composition]]) is:

$$
[T \circ S]_{\beta}^{\delta} = [T]_{\gamma}^{\delta}\ [S]_{\beta}^{\gamma}
$$

# Inverse Transformations and Isomorphism

_(observation)_

Let $T$ be an [[Isomorphism]].

- $T : V \rightarrow W$ is [[linear]]; $T^{-1} : W \rightarrow V$ is also linear.
- Let $\beta$ be a basis of $V$
- Let $\beta '$ be a basis of $W$

Then, the associated matrix to $T$ is:

$$
A = [T]_{\beta}^{\beta '}
$$

…and the associated matrix to $T^{-1}$ is its [[inverse matrix]]:

$$
A^{-1} = [T^{-1}]_{\beta '}^{\beta}
$$

Furthermore, let's remember that $T \circ T^{-1} = I_W$ and that $T^{-1} \circ T = I_V$ ([[Identity Transformation|identity transformations]]). With this, then we have that:

$$
[T]_{\beta}^{\beta '}\ [T^{-1}]_{\beta '}^{\beta} = [I_W]_{\beta '}^{\beta '} = I
$$

$$
[T^{-1}]_{\beta '}^{\beta}\ [T]_{\beta}^{\beta '}= [I_V]_{\beta}^{\beta} = I
$$

…where $I$ denotes the respective [[Identity Matrix|identity matrices]].
