---
date: 2022-08-23
type: 🧠
tags:
  - MAC/S3/MN1
---

**Topics:** [[Numerical Analysis]]

---

The _relative [[Error|error]]_ normalises the error to the true value. It's given by:

$$
E_{r} = \frac{|x-x_n|}{|x|}
$$

…where $x$ is the exact value we're trying to approximate to, while $x_n$ is our last approximation.

Compare the [[Absolute Error|absolute error]].

> [!warning]- If the Exact Value isn't Known
>
> If the exact value isn't known (i.e. we're using a [[Numerical Method|numerical method]] to find it), then $x$ is the last approximation we got, and $x_n$ the penultimate one.
>
> This can only be done with [[Convergence Order of a Numerical Method|convergent numerical methods]], since this ensures our last approximation is better than the one before.

# Relative Porcentual Error

The relative error can also be given the in a percentage ($E_r$%):

$$
\% E_{r} = \frac{|x-x_n|}{|x|}\ 100\%
$$
