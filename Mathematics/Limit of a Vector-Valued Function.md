---
date: 2023-02-08
type: 🧠
tags:
  - MAC/S4/C4
---

**Topics:** [[Vector-Valued Function]] - [[Calculus]]

---

_**(definition)**_

Let $r(t) : \mathbb{R} \to \mathbb{R}^n$ be a [[Vector-Valued Function|vector-valued function]] given by:

$$
r(t) = \langle r_1(t), r_2(t), \dots, r_n(t) \rangle
$$

We define the [[Limit|limit]] of $r(t)$ as $t$ approaches $a$ as:

$$
\lim_{t \to a} r(t) := \left\langle  \lim_{t \to a} r_1(t), \lim_{t \to a} r_2(t), \dots, \lim_{t \to a} r_n(t) \right\rangle
$$

…provided _all_ the indicated limits exist. If _any one of them_ fails to exist, then $\lim_{t \to a} r(t)$ _does not exist_.
