---
date: 2023-08-23
type: 🧠
tags:
  - MAC/5/E1
---

**Topics:** [[Measure of Shape]] - [[Statistics]]

---

_**(definition)**_

Given a [[Variable (Statistics)|variable]] $X$, its _skewness_ is a measure of how asymmetrical its data is with respect to its [[Arithmetic Mean|mean]].

Let $x_{1}, \dots, x_{n}$ be observations of the variable $X$. The _skewness_ of $X$ is defined as:

$$
\mathrm{Sk}(X) = \frac{1}{s^3} \left[ \frac{1}{n} \sum_{i=1}^n \left(x_{i} - \overline{X} \right)^3 \right]
$$

…where $s$ is $X$'s [[Standard Deviation|standard deviation]].

> [!tip]- Moments
> Notice that the second and third [[Moment|moment]] of $X$, which we'll denote by $m_{2}$ and $m_{3}$ respectively, are involved in this definition:
>
> $$
> \begin{align*}
> \mathrm{sk}(X) &= \frac{1}{s^3} (m_{3}) \\ &= \frac{m_{3}}{(m_{2})^{3/2}}
> \end{align*}
> $$

When skewness is negative, mass tends to be concentrated to the right of the mean (with a _tail_ on the left); when it's positive, it tends to be concentrated to its left (with a _tail_ on the right):

![[Skewness-1.png]]

([courtesy of Wikimedia Commons](https://commons.wikimedia.org/wiki/File:Negative_and_positive_skew_diagrams_(English).svg))

Negative and positive skew are sometimes referred to as _left-skewed_ and _right-skewed_, respectively.
