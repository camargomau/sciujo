---
date: 2023-05-12
type: 🧠
tags:
  - MAC/4/PB
---

**Topics:** [[Probability]] - [[Density Function of a Random Vector]]

---

_**(definition)**_

Let $(X,Y)$ be a [[Random Vector|random vector]].

The _marginal density function_ of $(X,Y)$ with respect to $X$ is defined as:

$$
f_X(x) = \sum_{y \in R_Y} f_{(X,Y)}(x,y)
$$

Similarly, the marginal density function of $(X,Y)$ with respect to $Y$ is defined as:

$$
f_Y(y) = \sum_{x \in R_X} f_{(X,Y)}(x,y)
$$

# Properties

1. $$ 0 \leq f_{(X,Y)}(x,y) \leq 1 $$

2. $$\sum_{x,y \in R_{(X,Y)}} f_{(X,Y)}(x,y) = 1$$
