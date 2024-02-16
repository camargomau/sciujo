---
date: 2023-02-21
type: 🧠
tags:
  - MAC/S4/PB
---

**Topics:** [[Combination]] - [[Combinatorics]]

---

When [[Combination|combining]] $k$ elements from a [[Set|set]] of $n$ elements (i.e. forming $k$ combinations, $k \leq n$), the number of combinations we can have is:

$$
\binom{n}{k} = \frac{n!}{k!(n-k)!}
$$

> [!tip]- Permutations divided by $k!$
> Notice that this is basically the formula for [[Permutations with no Repetitions|permutations with no repetitions]], but divided by $k!$.
>
> This is because each $k$-combination of a set of $n$ elements has $k!$ permutations, and when combining, we do not care about the order of the elements.

# Properties

_**(theorem)**_

When $k > n$, then:

$$
\binom{n}{k} = 0
$$

When $k = n$, then:

$$
\binom{n}{k} = 1
$$

When $k = 0$, then:

$$
\binom{n}{k} = 1
$$

When $k = 1$, then:

$$
\binom{n}{k} = n
$$
