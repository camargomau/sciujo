---
date: 2023-02-21
type: 🧠
tags:
  - MAC/S4/PB
---

**Topics:** [[Combinatorics]] - [[Probability]]

---

The _addition principle_ is a basic [[Counting Principle|counting principle]].

Intuitively, it tells us that if a situation can occur in $k$ different ways, and another situation (exclusive from the first one) can occur in $n$ different ways, then there are $n + k$ ways in which the first situation **or** the second one can occur.

> [!tip]- Or
> Notice that "or" is the keyword for addition. It tells us that we don't care specifically about which situation occurs; we only care if either of them occurs.
>
> Compare this with [[Multiplication Principle|multiplication]], which uses "and".

Mathematically, if $A$ and $B$ are two finite [[Disjoint Set|disjoint sets]], then:

$$
|A \cup B| = |A| + |B|
$$

> [!example]-
> Let's say we're shopping for shirts at two stores.
>
> In one store, we can choose from $5$ different colours of shirts. In the other store, we can choose from $4$ different colours.
>
> In total, we can choose from $5 + 4 = 9$ different colours.
