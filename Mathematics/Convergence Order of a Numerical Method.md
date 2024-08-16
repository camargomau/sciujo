---
date: 2022-08-25
type: 🧠
tags:
  - MAC/3/MN1
---

**Topics:** [[Numerical Analysis]] - [[Numerical Method]] - [[Limit of a Sequence]]

---

In many [[Numerical Method|numerical methods]], we calculate the first $n$ terms of a [[Sequence|sequence]] to observe a possible [[Limit of a Sequence|convergence]] to the final answer.

A [[Numerical Method|numerical method]] converges if:

$$
|x_{n} - x_{n-1}| < |x_{n-1}- x_{n-2}|
$$

That is, a numerical method converges if the difference between the last two approximations is always greater than or equal than the [[Absolute Error|absolute error]]. Notice that this difference is a [[Bound|bound]] for the absolute error.
