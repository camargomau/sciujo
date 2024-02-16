---
date: 2023-02-05
type: 🧠
tags:
  - MAC/S4/BD
---

**Topics:** [[Database]]

---

In databases, we have a _functional dependency_ when, in a [[Relation (database)|relation]], the [[Attribute Value|values]] in a set of [[Attribute|attributes]] are determined by the values in another set of attributes.

More formally, a functional dependency occurs between two attributes $X, Y$ in a relation if and only if each value of $X$ is associated with _exactly_ one (and only one) $Y$ value. We write such a functional dependency as $X \to Y$.

Indeed, it's called a functional dependency because it behaves just like a [[Function|function]]; it _is_ a function.
