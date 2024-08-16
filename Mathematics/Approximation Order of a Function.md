---
date: 2022-08-25
type: 🧠
tags:
  - MAC/3/MN1
---

**Topics:** [[Numerical Analysis]] - [[Function]]

---

Let $p(h)$ be a function that approximates another function $f(h)$$ (such as a [[Taylor Polynomial|Taylor polynomial]]).

Suppose that there exists a [[real number|real]] constant $M>0$, and a [[Natural Numbers|natural number]] $n$ such that:

$$
\frac{|f(h) - p(h)|}{|h^{n}|} \leq M
$$

…for a sufficiently small $h$. Then say that $p(h)$ approximates $f(h)$ with an _approximation order_ of $O(h^{n})$.

We denote this with:

$$
f(h) = p(h) + O(h^{n})
$$

$$
|f(h) - p(h)| \leq M|h_{n}|
$$

Notice that $O(h^{n})$ takes the place of $M|h^{n}|$, the error [[Bound|bound]].
