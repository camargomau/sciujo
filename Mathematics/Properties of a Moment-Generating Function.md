---
date: 2023-04-19
type: 🧠
tags:
  - MAC/S4/PB
  - MAC/S5/E1
---

**Topics:** [[Moment-Generating Function]] - [[Probability]]

---

_**(theorem)**_

1. $M_{Y}(t) = e^{ bt } M_{X}(at)$, where $Y = aX+b$

2. $M_{X}(t) = \sum_{n=0}^{\infty} \frac{t^n}{n!} \mathbb{E}[X^n]$

3. If $X$ and $Y$ are [[Event Independence|independent]] [[Random Variable|random variables]], then $M_{X+Y}(t) = M_{X}(t) M_{Y}(t)$.

	- But $M_{X+Y}(t) = M_{X}(t) M_{Y}(t) \centernot\implies X \perp\!\!\!\!\perp Y$

4. If $M_{X}(t) = M_{Y}(t)\ \forall t$, then $X$ and $Y$ have the same distribution (the same [[Density Function|density function]])

5. [[Moment-Generating Function of the Sum of the Random Variables in a Random Sample]]
