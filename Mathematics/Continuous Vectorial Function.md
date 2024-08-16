---
date: 2022-09-07
type: 🧠
tags:
  - MAC/3/C3
---

**Topics:** [[Continuous Function]] - [[Vectorial Function]]

---

_**(definition)**_

Let $f : \mathbb{R}^{n} \to \mathbb{R}^{m}$ be a [[Vectorial Function|vectorial function]]. We say that $f$ is _continuous_ in $\overline{x_{0}}$ if $\forall \varepsilon > 0$, $\exists \delta > 0$ such that:

$$
f(B_{\delta}(x_{0})) \subseteq B_{\varepsilon} (f(x_{0}))
$$

…(see [[Open Ball|open ball]]), or alternatively:

$$
\| f(\overline{x_{0}}) - f(\overline{x}) \| < \varepsilon
$$

…if $\| x_{0} - x \| < \delta$.

# Continuity in all $\mathbb{R}^n$

_**(theorem)**_

Let $f:\mathbb{R}^{n} \to \mathbb{R}^{m}$. $f$ is continuous in all $\mathbb{R}^n$ if and only if $f^{-1}(u)$ is open for all [[Open Set|open sets]] $u$ in $\mathbb{R}^{m}$.

> [!tip]- $f^{-1}(u)$
> $f^{-1}(u) = \{ x \in \mathbb{R}^{n}\ |\ f(x) \in u \}$.

# Composition

_**(corollary, from [[Continuous Function#Continuity in all mathbb R n|this theorem]])**_

If $f : \mathbb{R}^{n} \to \mathbb{R}^m$ and $g : \mathbb{R}^{k} \to \mathbb{R}^{n}$ are continuous, then $f \circ g : \mathbb{R}^{k} \to \mathbb{R}^m$ is also continuous.
