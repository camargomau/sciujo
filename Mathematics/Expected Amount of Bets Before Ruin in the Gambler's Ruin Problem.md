---
date: 2024-04-04
type: 🧠
tags:
  - MAC/6/PE
---

**Topics:** [[Gambler's Ruin Problem]]

---

Say we are interested in knowing the expected amount of bets before player A will get ruined in the [[Gambler's Ruin Problem|gambler's ruin problem]].

_**(theorem)**_

This is given by:

$$
m_{K} =
\begin{cases}
N(N-K) &\text{if } p=q=\frac{1}{2} \\[1em]
\left( \frac{1}{q-p} \right) \left( K - N \left[ \frac{ 1-\left( \frac{q}{p} \right)^K }{1-\left( \frac{q}{p} \right)^N} \right]  \right)  &\text{if } p \neq q \neq \frac{1}{2}
\end{cases}
$$

