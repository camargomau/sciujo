---
date: 2022-08-18
type: 🧠
tags:
  - MAC/3/MD
---

**Topics:** [[Discrete Mathematics]] - [[Algebra]]

---

_**(definition)**_

A relation is a [[Set|set]] in which all pairs are ordered. When two elements of the set are related, we write $aRb$ or $(a,b) \in R$.

> [!example]-
>
> Let $A = B = \{1, 2, 3, 4, 5, 6\}$ and let $R = \{(a, b)\ :\ a|b \}$ (remember that $a | b$ if $\exists\ x \in \mathbb{Z}$ such that $b = ka$).
>
> Thus, we have that $R = \{(1,1), (1,2), (1,3), (1,4), (1,5), (1,6), (2, 2), (2, 4), (2, 6), (3, 3), (3, 6), (4, 4), (5, 5), (6, 6)\}$.

_**(definition)**_

Let $A, B$ be sets. A relation of $A$ in $B$ is a subset of $A \times B$ ([[Cartesian Product]]).

$R \text{ is a relation } \iff R \subseteq A \times B$

> [!example]-
>
> Let $C = \{ \text{capital cities of the world} \}$ and $A = \{ \text{countries of the world} \}$. Let $R$ be the relation where $x \in C$ is the capital city of $y \in A$. For instance:
>
> $(\text{CDMX}, \text{Mexico}) \in R$
> $\text{CDMX}\ R\ \text{Mexico}$
>
> …but $(\text{Guadalajara}, \text{Mexico}) \notin R$.
>
> Note that that $\{ \text{All countries and its capital cities} \} \subseteq C \times A$. With this, we can say that that:
>
> $R = \{(a, b) \mid a \text{ is the capital city of } b \} \subseteq C \times A$

_**(lemma)**_ ^a3af3d

If $R$ is a relation, then $\{(y,x) \mid (x,y) \in R \}$ is also a relation.

> [!abstract]- Proof
> We have that $(y,x)$ is an ordered pair. Then, $\{(y,x) \mid (x,y) \in R \}$ is a set of ordered pairs. Therefore, it's a relation.
