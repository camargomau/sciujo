---
date: 2023-03-20
type: 🧠
tags:
  - MAC/S4/PB
---

**Topics:** [[Distribution Function]] - [[Probability]]

---

_**(definition)**_

In [[Distribution Function]], we defined what $F_X(x)$ is; we defined a distribution function $F_X$ _exactly at_ $x \in \mathbb{R}$.

Now, we'll define _$F_X$ at $x$ **from the left**_, denoted $F_X(x_-)$, as:

$$
F_X(x_-) := \lim_{y \to x} F_X(y)
$$

_**(theorem)**_

Notice that:

$$
F_X(x_-) = \mathbb{P}(X < x)
$$

…which is very similar to the normal definition of $F_X(x)$, but with $<$ instead of $\leq$. As such, it is common to find $F_x(x)$ expressed in this form.
