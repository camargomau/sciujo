---
date: 2023-02-06
type: 🧠
tags:
  - MAC/4/BD
---

**Topics:** [[Database]]

---

In databases, we say that a [[Relation (database)|relation]] (table) has a _transitive dependency_ if, for three distinct sets of [[Attribute|attributes]] $A$, $B$ and $C$ we have that:

1. $A \to B$ ($B$ is [[Functional Dependency|functionally dependant]] on $A$)
2. $B \not \to A$ ($A$ is not functionally dependant on $B$)
3. $B \to C$

The resulting functional dependency $A \to C$ is what we call a _transitive dependency_. Normally we'll refer to transitive dependencies where $A$ is a [[Candidate Key|candidate key]] (or [[Primary Key|primary key]]).

Transitive dependencies are to be avoided if we want to have a relation in the [[Third Normal Form|third normal form]].
