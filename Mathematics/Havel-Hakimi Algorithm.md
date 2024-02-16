---
date: 2023-02-09
type: 🧠
tags:
  - MAC/S4/TG
---

**Topics:** [[Graph Theory]]

---

The _Havel-Hakimi algorithm_ is an algorithm that lets us know if there exists a [[Simple Graph|simple graph]] whose [[Vertex Degree|degree sequence]] is a given [[Increasing and Decreasing Sequence|non-increasing]] [[Sequence|sequence]] of non-negative [[Integer|integers]].

The algorithm consists of the following steps:

1. Take the first greatest integer. Let $n$ be this value.
2. Remove $n$ from the sequence
3. Subtract $1$ from the next $n$ integers.
4. Reorder the sequence so that it is non-increasing again.
5. Repeat steps 1 through 4 until we reach a sequence that consists of all zeroes or we get a negative integer.

When the resulting sequence consists of all zeroes, the sequence corresponds to a simple graph and we say that it is a _graphic_ sequence. Otherwise, the sequence doesn't correspond to a simple graph and we say that it is _non-graphic_.

> [!example]- Graphic Example
> Let $\{ 5, 4, 3, 2, 2, 2, 2, 2 \}$ be our sequence. By following the algorithm, we get:
>
> 1. First iteration:
> 	1. $n=5$
> 	2. $\{ \cancel{5}, \mathbf{4, 3, 2, 2, 2}, 2, 2 \}$
> 	3. $\{ \mathbf{3, 2, 1, 1, 1}, 2, 2 \}$
> 	4. $\{ 3, 2, 2, 2, 1, 1, 1 \}$
> 2. Second iteration:
> 	1. $n = 3$
> 	2. $\{ \cancel{3}, \mathbf{2, 2, 2}, 1, 1, 1 \}$
> 	3. $\{ \mathbf{1, 1, 1}, 1, 1, 1 \}$
> 	4. $\{ 1, 1, 1, 1, 1, 1 \}$
> 3. Third iteration:
> 	1. $n = 1$
> 	2. $\{ \cancel{1}, \mathbf{1}, 1, 1, 1, 1 \}$
> 	3. $\{ \mathbf{0}, 1, 1, 1, 1 \}$
> 	4. $\{ 1, 1, 1, 1, 0 \}$
> 4. Fourth iteration:
> 	1. $n=1$
> 	2. $\{ \cancel{1}, \mathbf{1}, 1, 1, 0 \}$
> 	3. $\{ \mathbf{0}, 1, 1, 0 \}$
> 	4. $\{ 1, 1, 0, 0 \}$
> 5. Fifth iteration:
> 	1. $n=1$
> 	2. $\{ \cancel{1}, \mathbf{1}, 0, 0 \}$
> 	3. $\{ \mathbf{0}, 0, 0 \}$
> 	4. $\{ 0, 0, 0 \}$
>
> Voilà. Since the resulting sequence consists of all zeroes, the sequence **is graphic**. In effect, its associated simple graph is the following:
>
> ![[Havel-Hakimi Algorithm-1.png]]
