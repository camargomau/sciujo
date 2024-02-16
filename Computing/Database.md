---
type: 🗺
---

A _database_ is a collection of data that is organised structurally according to a specific well-defined set of rules.

# Database Structure

A database is made up of [[Relation (database)|relations]], which we informally refer to as _tables_. What we informally call _columns_ are its [[Attribute|attribute]], which contain specific [[Attribute Value|values]]. On the other hand, its [[Tuple|tuples]] are what we refer to when we say _records_ or _rows_.

# Keys and Dependency

The concept of _keys_ is important in databases:

- A [[Superkey|superkey]] is a set of attributes that identifies each tuple in a relation.
- A [[Candidate Key|candidate key]] is the minimal of the superkeys (whether the only one or one among many).
- A [[Primary Key|primary key]] is the candidate key we choose to identify a tuple.
- A [[Foreign Key|foreign key]] is a primary key of a relation included within another relation.

Given the nature of keys, the concept of _dependency_ arises:

- A [[Functional Dependency|functional dependency]] is an attribute value dependency that behaves just like a [[Function|function]].
- A [[Partial Dependency|partial dependency]] is a functional dependency where only a part of the candidate key determines the values in another attribute.
- A [[Transitive Dependency|transitive dependency]] is a functional dependency where an attribute is dependant on a key by means of another attribute (indirectly, not directly).

# Database Normalisation

To avoid errors and anomalies, it is desirable to [[Database Normalisation|normalise]] a database. This normalisation is carried out by making all the relations in a database be compliant with the so-called _normal forms_:

1. The [[First Normal Form|first normal form]] requires all the attribute values to be atomic.
2. The [[Second Normal Form|second normal form]] requires to have no partial dependencies.
3. The [[Third Normal Form|third normal form]] requires to have no transitive dependencies.
