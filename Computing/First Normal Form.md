---
date: 2023-02-05
type: 🧠
tags:
  - MAC/S4/BD
aliases:
  - 1NF
---

**Topics:** [[Database]] - [[Database Normalisation]]

---

When normalising a database, we say that a [[Relation|relation]] (table) is in the _first normal form_ (1NF) if it satisfies the following 3 conditions:

1. Each [[Attribute|attribute]] (column) is atomic. That is, it contains one and only one [[Attribute Value|value]] for each [[Tuple|tuple]].
2. The values stored in a given [[Attribute|attribute]] are of the same nature (same domain, same data type).
3. All the attributes have unique names
