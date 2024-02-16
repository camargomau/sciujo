---
date: 2023-02-05
type: 🧠
tags:
  - MAC/S4/BD
---

**Topics:** [[Database]] - [[Database Normalisation]]

---

When normalising a database, we say that a [[Relation (database)|relation]] (table) is in the _second normal form_ (2NF) if it satisfies the following two conditions:

1. It's in the [[First Normal Form|first normal form]]
2. It has no [[Partial Dependency|partial dependencies]]

In other words, a relation is in 2NF if it is in 1NF and additionally every [[Non-Prime Attribute|non-prime attribute]] depends on the whole of every [[Candidate Key|candidate key]].
