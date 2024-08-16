---
date: 2023-08-23
type: 🧠
tags:
  - MAC/5/E1
---

**Topics:** [[Measure of Association]] - [[Statistics]]

---

_**(definition)**_

Let $(x_{1}, y_{1}), \dots, (x_{n}, y_{n})$ be observations of the [[Variable (Statistics)|variables]] $(X,Y)$.

_Pearson's correlation coefficient_ between the variables $(X,Y)$ is defined as:

$$
\mathcal{r}_{XY} = \frac{S_{XY}}{S_{X}S_{Y}}
$$

…where $S_{XY}$ is the [[Covariance|covariance]] of $(X,Y)$, and $S_{X}, S_{Y}$ are the [[Standard Deviation|standard deviations]] of $X$ and $Y$, respectively.

# Properties

- $\mathcal{r}_{XY} \in [-1, 1]$
- If $x \perp\!\!\!\!\perp y$, $\mathcal{r}_{XY} = 0$
- If $\mathcal{r}_{XY} < 0$, there's an inverse relation between the variables (i.e. when one variable grows, the other decreases)
