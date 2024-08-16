---
date: 2023-03-22
type: 🧠
tags:
  - MAC/4/PB
---

**Topics:** [[Distribution Function]] - [[Probability Measure]] - [[Probability]]

---

_**(theorem)**_

Let $X$ be a [[Random Variable|random variable]], $a \in \mathbb{R}$ and $F_X$ a [[Distribution Function|distribution function]].

From the [[Distribution Function|definition of a distribution function]] at $a$ (denoted $F_X(a)$) and the definition of a distribution function at $a$ [[Distribution Function From the Left|from the left]] (denoted $F_X(a_-)$), we get that:

1. $\mathbb{P}(X \leq a) = F_X(a)$
2. $\mathbb{P}(X > a) = 1 - F_X(a)$
3. $\mathbb{P}(X < a) = F_X(a_-)$
4. $\mathbb{P}(X \geq a) = 1 - F_X(a_-)$

And that:

1. $\mathbb{P}(a < X \leq b) = F_X(b) - F_X(a)$
2. $\mathbb{P}(a \leq X \leq B) = F_X(b) - F_X(a_-)$
3. $\mathbb{P}(a \leq X < b) = F_X(b_-) - F_X(a_-)$
4. $\mathbb{P}(a < X < b) = F_X(b_-) - F_X(a)$

Additionally:

1. $\mathbb{P}(X = a) = F_X(a) - F_X(a_-)$

Note that the distribution function is continuous at $x$ if and only if $\mathbb{P}(X = x) = 0$ .
