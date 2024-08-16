---
date: 2023-02-21
type: 🧠
tags:
  - MAC/4/PB
---

**Topics:** [[Permutation]]

---

If we select $k$ objects from a [[Set|set]] of $n$ **distinct** elements, and we **cannot** repeat our selection, then the number of [[Permutation|permutations]] we can have is:

$$
{}_n\text{P}_k = \frac{n!}{(n-k)!}
$$

For a set with subsets of equal elements, see [[Permutations with Groups of Equal Elements|permutations with groups of equal elements]].

> [!example]-
> _How many permutations can be made with the letters of the word "COLUMN"?_
>
> Since "COLUMN" has 6 letters and it contains no repeated letters, then we can have ${}_6\text{P}_6 = 6! = 720$ permutations.
>
> _How many 4-letter permutations can be made with the letters of the word "COLUMN"?_
>
> This time, we can have ${}_6\text{P}_6 = \frac{6!}{(6-4)!} = \frac{6!}{2!} = 6(5)4(3) = 360$ permutations.
