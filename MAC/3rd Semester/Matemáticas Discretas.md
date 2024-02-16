---
type: 🏫
tags:
  - MAC/S3/MD
---

# Sets

When we have two sets, we can define their [[Cartesian Product|Cartesian product]].

The [[Partition of a Set|partition of a given set]] is a set that contains subsets of the set that are non-overlapping and whose union is the whole set.

# Relations

[[Relation|Relations]] can have [[Properties of Relations|several properties]].

Relations can be represented as a [[Matrix of a Relation|matrix]] or a [[Digraph|digraph]]. The properties of relations can be [[Properties of Relations in their Representations|easily determined]] from these representations.

Relations can be [[Composition of Relations|composed with each other]]. When a relation is composed with itself, we call it a [[Powers of a Relation|power]].

There are several types of relations:

- [[Function|Functions]], our good friends from calculus

- [[Equivalence Relation|Equivalence relations]], a type of relation that allows us to define equivalences
	- [[Equivalence Class|Equivalence classes]] can be built from these type of relations
	- [[Quotient Set|Quotient sets]] can also be build from these type of relations

- [[Order Relation]], a type of relation that allows us to define an order within a set
	- Order relations can be [[Partially Ordered Set|partial]] or [[Total Order Relation|total]]
	- [[Well-Order|Well-orders]] are a specific type of total order relation

# Partially Ordered Sets

[[Partially Ordered Set|Partially ordered sets]] (or poset, for short) are sets with a partial order relation.

There are several kinds of "boundary" elements we can find in a poset:

- The [[Minimal and Maximal]] (and their [[Absolute Minimal and Maximal Elements|absolute versions]]) refer to "least" and "greatest" elements in the poset (i.e. those that aren't preceded or succeeded by another element)
- The [[Upper and Lower Bounds]] refer to the elements in the poset that _bound_ a subset of the poset (i.e. precede or succeed _all_ the elements of the subset)
	- The [[Minimum and Maximum]] (not to be confused with minimal and maximal) refer to the upper/lower bounds of a subset that are also within that same subset
	- The [[Supremum and Infimum]] refer to the "least"/"greatest" upper/lower bounds in the whole poset

> [!tip]- Minimal/Maximal and Minimum/Maximum
> It is important to differentiate between minimal/maximal and minimum/maximum.
>
> As a way to remember which one is which, I focus on their ending: minimal/maximal, which end with "-al", refer to the "least" and "greatest" elements in _all_ the poset, while the minimum/maximum merely refer to the bounds of a subset that are within said subset.

Posets can be represented with [[Hasse Diagram|Hasse diagrams]], which can be seen as simplified digraphs.

# Lattices

Posets where every subset of two elements has a _unique_ supremum and a unique infimum are called [[Lattice|lattices]].
