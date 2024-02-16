---
date: 2023-02-06
type: 🧠
tags:
  - MAC/S4/BD
---

**Topics:** [[Database]]

---

In databases, we say that a [[Relation (database)|relation]] (table) has a _partial dependency_ if there exists a [[Non-Prime Attribute|non-prime attribute]] that is [[Functional Dependency|functionally dependant]] on only a part of _any_ [[Candidate Key|candidate key]].

For example, if a candidate key in our relation is made up of 2 attributes, and there exists a non-prime attribute that only depends on one of these 2 attributes, then the relation has a partial dependency.

Partial dependencies are to be avoided if we want to have a relation in the [[Second Normal Form|second normal form]].
