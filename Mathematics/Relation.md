---
date: 2021-11-30
type: 🧠
tags:
  - MAC/S1/ÁS
  - MAC/S3/MD
aliases:
  - relation
---

**Topics:** [[Discrete Mathematics]] - [[Algebra]]

---

A (binary) relation associates elements of one set with elements of another (or the same) set.

There are three types of relations:

- [[Function|Functions]]
- [[Equivalence Relation|Equivalence relations]]
- [[Order Relation|Order relations]]

Relations [[Relations as a Set|can also be seen as a set]]. They have a [[Domain and Range of a Relation|domain and a range]]. Relations can have several [[Properties of Relations|properties]] and they can also have [[Inverse Relation|inverses]]. Relations can be represented graphically with a [[Digraph|digraph]], and they can also be represented with a [[Matrix of a Relation|matrix]].

# Examples

> [!example]- Trivial Examples
> Examples of trivial binary relations are "greater than" ($\geq$), "equal to" ($=$) or "less than" ($\leq$). Notice how these relations establish an association between two (and only two) elements of two sets.

> [!example]- Example 1
> Let $A = B = \{a, b\}$. We have that:
>
> $$
> A \times B = \{(a,a), (a,b), (b,a), (b,b)\}
> $$
>
> There are $2^{4}=16$ possible relations in $A \times B$:
>
> - $R_{1}=\varnothing$
> - $R_{2}=\{(a,a)\}$
> - $R_{3}=\{(a,b)\}$
> - $R_{4}=\{(b,a)\}$
> - $R_{5}=\{(b,b)\}$
> - $R_{6}=\{(a,a), (a,b)\}$
> - $R_{7}=\{(a,a), (b,a)\}$
> - $R_{8}=\{(a,a), (b,b)\}$
> - $R_{9}=\{(a,b), (b,a)\}$
> - $R_{10}=\{(a,b), (b,b)\}$
> - $R_{11}=\{(b,a), (b,b)\}$
> - $R_{12}=\{(a,a), (a,b), (b,a)\}$
> - $R_{13}=\{(a,a), (a,b), (b,b)\}$
> - $R_{14}=\{(a,a), (b,a), (b,b)\}$
> - $R_{15}=\{(a,b), (b,a), (b,b)\}$
> - $R_{16}=A \times B$
>
> We can say the following about some of these relations:
>
> $$
> \text{dom}(R_{6})=\{a\}
> $$
>
> $$
> \text{ran}(R_{6})=\{a,b\}
> $$
>
> $$
> R^{-1}_{12} = \{(a,a), (b,a), (a,b)\} = R_{12}
> $$
>
> $$
> R^{-1}_{13} = \{(a,a), (b,a), (b,b)\} \neq R_{13}
> $$

> [!example]- Example 2
> Let $X = \{2, 3, 4\}$, $Y=\{3,4,5,6,7\}$. We define the relation $R$ as:
>
> $$
> (x,y) \in R \text{ if } x \text{ divides } y
> $$
>
> The relation seen as a set is:
>
> $$
> R = \{(2,4), (2,6), (3,3), (3,6), (4,4)\}
> $$
>
> …and we can also see that:
>
> $$
> \text{dom}(R)=\{2,3,4\}
> $$
>
> $$
> \text{ran}(R)=\{3,4,6\}
> $$
