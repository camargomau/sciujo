---
date: 2022-08-30
type: 🧠
tags:
  - MAC/3/MN1
---

**Topics:** [[Discrete Mathematics]] - [[Relation]]

---

_**(definition)**_

Let $R \subseteq X \times Y$ and $S \subseteq Y \times Z$ be two [[Relation|relations]].

The composition of $R$ and $S$, denoted $R \circ S$, is the relation:

$$
R \circ S = \{ (x,z) \in X \times Z \mid \exists y\in Y : (x,y) \in R \land (y,z) \in S \}
$$

In other words, $R \circ S \subseteq X \times Z$ is defined by the rule that says that $(x,z) \in R$ if and only if there is an element $y \in Y$ such that $(x,y) \in R$ and $(y,z) \in S$.

# Associativity

_**(theorem)**_

Let $A, B, C, D$ be [[Set|sets]]. Let $R_{1} \subseteq A \times B$, $R_{2} \subseteq B \times C$ and $R_{3} \subseteq C \times D$ (see [[Cartesian Product]]).

Then, it's true that:

$$
R_{1} \circ (R_{2} \circ R_{3}) = (R_{1} \circ R_{2}) \circ R_{3}
$$
