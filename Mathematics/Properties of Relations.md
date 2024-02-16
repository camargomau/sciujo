---
date: 2022-08-18
type: 🧠
tags:
  - MAC/S3/MD
aliases:
  - reflexive property
  - symmetric property
  - antisymmetric property
  - transitive property
---

**Topics:** [[Discrete Mathematics]] - [[Relation]]

---

_**(definition)**_

A given [[Relation|relation]] $R$ in a set $A$ is:

- **Reflexive** if and only if $aRa \quad \forall\ a \in A$
- **Symmetric** if and only if $aRb \iff bRa \quad \forall\ a, b \in A$
- **Antisymmetric** if and only if $aRb \land bRa \implies a=b$
- **Transitive** if and only if $aRb \land bRc \implies aRc \quad \forall\ a,b,c \in A$

The properties of a given relation can be easily determined [[Properties of Relations in their Representations|with the help of its digraph and matrix]].

> [!example]- Example 1
> Let $A = \{a, b, c, d\}$ and:
>
> $R = \{(a,a), (a,b), (a,c), (b,a), (b,b), (b,c), (b,d), (d,d)\}$
>
> Notice that:
>
> - $R$ isn't reflexive since $c \not R c$
> - $R$ isn't symmetric since $aRc$ but $c \not R a$
> - $R$ isn't antisymmetric since $aRb$ and $bRa$ but $a \neq b$
> - $R$ isn't transitive since $aRb$ and $bRd$ but $a \not R d$

> [!example]- Example 2
> Let $A = \mathbb{R}$. Let $R$ be the relation defined by $x \leq y$ if $x, y \in \mathbb{R}$.
>
> Notice that:
>
> - $R$ is reflexive since $x \leq x$ $\forall x \in \mathbb{R}$
> - $R$ isn't symmetric since $1 \leq 2 \;\not\!\!\!\implies 2 \leq 1$
> - $R$ is antisymmetric since $x \leq y \land y \leq x \implies x = y$.
> - $R$ is transitive since $x \leq y \land y \leq z \implies x \leq z$
