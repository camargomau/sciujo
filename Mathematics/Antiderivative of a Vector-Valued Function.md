---
date: 2023-02-13
type: 🧠
tags:
  - MAC/4/C4
---

**Topics:** [[Vector-Valued Function]] - [[Derivative of a Vector-Valued Function]]

---

_**(definition)**_

Let $r : \mathcal{D}_1 \subseteq \mathbb{R} \to V_n$ be a [[Vector-Valued Function|vector-valued function]] and $r' : \mathcal{D}_2 \subseteq \mathbb{R} \to V_n$ its [[Derivative of a Vector-Valued Function|derivative]].

We will define the following function as the _antiderivative_ (or _primitive function_) of $r'$:

$$
\int r'\ dt := r + \vec c
$$

Note that $\vec c \in V_n$ (it's a [[Vector|vector]]).

_**(theorem)**_

Given $r(t) = \langle r_1(t), \dots, r_n(t) \rangle$, then:

$$
\int r\ dt = \left\langle \int r_1\ dt,\ \dots, \int r_n\ dt \right\rangle
$$
