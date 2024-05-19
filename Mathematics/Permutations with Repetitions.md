---
date: 2023-02-21
type: 🧠
tags:
  - MAC/S4/C4
---

**Topics:** [[Permutation]]

---

If we select $k$ objects from a [[Set|set]] of $n$ distinct elements, and we **can** repeat our selection, then the number of [[Permutation|permutations]] we can have is simply:

$$
{}_n\text{PR}_k = n^k
$$

> [!example]-
> Let's say we are trying to calculate the amount of licence plates we can have when each plate contains $3$ letters and $4$ digits.
>
> For the letters, considering an [[Alphabet|alphabet]] of 26 letters, we can have ${}_{26}\text{PR}_3 = 26^3 = 17\ 576$ different permutations.
>
> For the digits, we can have ${}_{10}\text{PR}_3 = 10^4 = 10\ 000$ different permutations.
> 
> Now, since we're choosing 3 letters **and** 4 digits, the number of total permutations is given by the [[Multiplication Principle|multiplication principle]]:
>
> $$
> \text{Total Permutations} = 17\ 576(10\ 000) = 175\ 760\ 000
> $$
