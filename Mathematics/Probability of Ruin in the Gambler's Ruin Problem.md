---
date: 2024-04-04
type: 🧠
tags:
  - MAC/6/PE
---

**Topics:** [[Gambler's Ruin Problem]]

---

Say we are interested in knowing the probability of player A getting ruined in the [[Gambler's Ruin Problem|gambler's ruin problem]].

_**(observation)**_

Let $\gamma$ be the first moment upon which the previously defined process reaches one of its two absorbing states ($0$ and $N$). That is:

$$
\gamma = \min \left\{ n \geq 0 \mid X_{n} = 0  \vee X_{n} = N \right\}
$$

Then, the probability of player A getting ruined is given by:

$$
U_{K} = \mathbb{P}(X_{\gamma} = 0 \mid X_{0} = K)
$$

_**(theorem)**_

More specifically, we can deduce that:

$$
U_{K} =
\begin{cases}
\dfrac{N-K}{K} &\text{if } p=q=\frac{1}{2} \\[1em]
\dfrac{\left( \frac{q}{p} \right)^{K}-\left( \frac{q}{p} \right)^{N}}{1-\left( \frac{q}{p} \right)^{N}} &\text{if } p \neq q \neq \frac{1}{2}
\end{cases}
$$
