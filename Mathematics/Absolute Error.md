---
date: 2022-08-23
type: 🧠
tags:
  - MAC/3/MN1
---

**Topics:** [[Numerical Analysis]]

---

The _absolute [[Error|error]]_ is the distance between the exact value and the approximate value. It's given by:

$$
E_{a} = | x - x_{n} |
$$

Compare the [[Relative Error|relative error]].

> [!warning]- If the Exact Value isn't Known
>
> If the exact value isn't known (i.e. we're using a [[Numerical Method|numerical method]] to find it), then $x$ is the last approximation we got, and $x_n$ the penultimate one.
>
> This can only be done with [[Convergence Order of a Numerical Method|convergent numerical methods]], since this ensures our last approximation is better than the one before.
