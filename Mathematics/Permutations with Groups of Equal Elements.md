---
date: 2023-02-21
type: 🧠
tags:
  - MAC/4/PB
---

**Topics:** [[Permutation]]

---

Let's say we have a [[Set|set]] of $n$ elements with group of **equal** elements. We have $n_1$ elements of type 1, $n_2$ elements of type 2, etc. ($n = n_1 + n_2 + \dots + n_k$).

In such a case, the number of _distinguishable_ [[Permutation|permutations]] we can form with the $n$ elements is:

$$
{}_n\text{P}_{n_1, \dots, n_k} = \frac{n!}{n_1!n_2!\dots n_k!}
$$

For a set whose elements are all distinct, see [[Permutations with no Repetitions|permutations with no repetitions]].

> [!example]-
> _How many permutations can be made with the letters of the word "PEPPER"?_
>
> Notice that "PEPPER" has 6 letters:
> - $3$ Ps
> - $2$ Es
> - $1$ R
>
> Thus, we can have ${}_6\text{P}_3,2,1 = \frac{6!}{3!2!1!} = \frac{6(5)4}{2} = 60$ permutations.
