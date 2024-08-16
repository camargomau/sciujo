---
date: 2022-08-11
type: 🧠
tags:
  - MAC/3/MD
---

**Topics:** [[Discrete Mathematics]]

---

_**(definition)**_

Let $X, Y$ be finite [[sets]]. We define the _Cartesian product_ of $X$ and $Y$, denoted by $X \times Y$, in the following way:

$$
X \times Y = \{ (x, y) \mid x \in X,\ y \in Y \}
$$

If $X = Y$, then $X \times X$ may be denoted as $X^2$, but be careful to not confuse this with the [[squared]] $X$ set.

> [!tip]- Empty Sets
> - If $X$, $Y$ or both are empty, then $X \times Y = \varnothing$.
> - If $X, Y$ are non-empty, then we have that $X \times Y = Y \times X$ if and only if $X = Y$.

# Multiple Sets

If $X_1, \dots, X_n$ are non-empty sets, then:

$$
X_1 \times \dots \times X_n = \{ (x_1, \dots, x_i) \mid x_i \in X_i, i = 1, \dots, n \}
$$

We call $(x_1, \dots, x_i)$ an _n-uple_.

> [!example]-
>
> Let $A = \{ 1, 2 \}$, $X = \{a, b\}$, $Y = \{ \alpha, \beta \}$. Then:
>
> $$
> A \times X \times Y = \{ 1, a, \alpha), (1, a, \beta),
> $$
>
> $$
> (1, b, \alpha), (1, b, \beta),
> $$
>
> $$
> (2, a, \alpha), (2, a, \beta),
> $$
>
> $$
> (2, b, \alpha), (2, b, \beta) \}
> $$

# Cardinality

Let $X, Y$ be finite sets such that $|X| = n$ and $|Y| = m$ ([[Cardinality|cardinality]]). Then, we have that:

$$
|X \times Y | = |X| \cdot |Y|
$$

…and in general:

$$
|X_1 \times \dots \times X_n| = |X_1| \cdot \times \cdot |X_n|
$$

> [!example]-
>
> Let $A = \{ a, b, c, d \}$, $X = \{x, y, z\}$, $Y = \{y, z, t\}$. Note that $X \cap Y = \{y, z\}$. Then, we have that:
>
> $$
> A \times (X \cap Y) = \{ (a,y), (a,z), (b,y), (b,z), (c,y), (c,z), (d,y), (d,z) \}
> $$
>
> We also have that:
>
> $$
> A \times X = \{ (a,x), \dots, (d,z) \}
> $$
>
> $$
> A \times Y = \{ (a,y), \dots, (d,t) \}
> $$
>
> …and that:
>
> $$
> (A \times X) \cap (A \times Y) = \{ (a,y), \dots, (d,t) \}
> $$
>
> Note that $(A \times X) \cap (A \times Y) = A \times (X \cap Y)$.

# Distributivity

Notice that the last part of the previous example tells us that the Cartesian product is distributive with respect to [[intersection]]. That is:

$$
A \times (X \cap Y) = (A \times X) \cap (A \times Y)
$$

$$
(X \cap Y) \times A = (X \times A) \cap (Y \times A)
$$

It's also true that the Cartesian product is distributive with respect to [[union]]:

$$
A \times (X \cup Y) = (A \times X) \cup (A \times Y)
$$

$$
(X \cup Y) \times A = (X \times A) \cup (Y \times A)
$$
