---
date: 2022-08-25
type: 🧠
tags:
  - MAC/S3/MN1
---

**Topics:** [[Numerical Analysis]] - [[Numerical Method]]

---

Any given a [[Numerical Method|numerical method]] can be said to be stable or non-stable.

Let $E_n$ denote the growth of the [[Error|error]] after $n$ subsequent operations, and $\xi$ denote the error in any given step of the calculations.

Then:

- If $|E(n)| \approx C_{n}\xi$, we say that the error growth is _linear_ ($C$ being a constant that's independent from $n$)
	- We call a method with a linear error growth a **stable method**
- If $|E(n)| \approx k^{n} \xi$ for a given $k > 1$, the growth of the error is _exponential_
	- We call a method with an exponential error growth an **unstable method**

> [!tip]- Things to Consider
> Most of the time, a linear error growth is inevitable. When $C$ and $\xi$ are small, the results of the method are generally acceptable.
>
> An exponential error growth should be avoided, since $k^n$ will be big even for small values of $n$. This results in unacceptable inaccuracies.
