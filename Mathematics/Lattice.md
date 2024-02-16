---
date: 2022-09-20
type: 🧠
tags:
  - MAC/S3/MD
---

**Topics:** [[Discrete Mathematics]]

---

_**(definition)**_

Let $(L, \preceq)$ be a [[Partially Ordered Set|poset]].

$(L, \preceq)$ is a _lattice_ if and only if every subset $\{a, b\} \subseteq L$ has [[Supremum and Infimum|a unique supremum and a unique infimum]].

# $\lor$ and $\land$

In a lattice, we define two operations $\lor$ and $\land$ as follows:

$$
a \lor b := \sup\{a,b\}
$$

$$
a \land b := \inf\{a,b\}
$$

# Examples

> [!example]- Examples of $a \lor b$ and $a \land b$
> In the "less or equal to" relation ($\leq$):
>
> - $a \lor b = \max\{a,b\}$
> - $a \land b = \min\{a,b\}$
>
> In the "divisibility" relation ($|$):
>
> - $a \lor b = \text{mcm}(a,b)$
> - $a \land b = \text{MCD}(a,b)$
>
> In the "inclusion" relation ($\subseteq$):
>
> - $a \lor b = a \cup b$
> - $a \land b = a \cap b$

> [!example]- Lattice Example 1
> $(\mathbb{N}, \leq)$ is a lattice.
>
> We have that:
> - $a \lor b = \max\{a,b\}$
> - $a \land b = \min\{a,b\}$

> [!example]- Lattice Example 2
> Let $X = \{1,2,3\}$ and $L = \mathcal{P}(x)$ ([[Power Set|power set]]).
>
> $(\mathcal{P}(X), \subseteq)$ is a lattice.
>
> Furthermore, [[Power Set Lattices|this is true for any set]] $X$, irrespective of its [[Cardinality|cardinality]] or nature of elements.

> [!tip]- All Totally Ordered Sets are Lattices
> Notice that all [[Total Order Relation|totally ordered sets]] are lattices.
