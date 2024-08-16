---
date: 2022-08-22
type: 🧠
tags:
  - MAC/3/C3
---

**Topics:** [[Calculus]] - [[Topology]]

---

_**(definition)**_

Let $A \in \mathbb{R}^n$. We say that $A$ is _closed_ if and only if $A^c$ (its [[Complement Set|complement]]) is [[Open Set|open]].

> [!tip]- Closed does not imply not Open
>
> Remember that a set being closed doesn't imply it's not open. Similarly, a set being open doesn't imply it's not closed.
>
> The [[Empty Set|empty set]] is an example of a set that is closed _and_ open at the same time.

> [!example]- Example 1
> Let $A \subseteq \mathbb{R}$, $A = [0, 1]$.
>
> We have that $A^{c}= (-\infty, 0) \cup (1, \infty)$. Notice that $A^{c}$ is open, so it follows that $A$ is closed.

> [!example]- Example 2
> Let $B = [2, 3)$.
>
> We have that $B^{c} = (\infty, 2) \cup [3, \infty)$. Notice that $B^c$ isn't open, so it follows that $B$ isn't closed.
>
> Notice that $B$ also isn't open (but this doesn't follow the closeness of $B^c$).

> [!example]- Example 3
> Let $C = (-\infty, 0)$.
>
> We have that $C^{c} = [0, \infty)$. Notice that $C^c$ isn't open, so it follows that $C$ isn't closed. However, do notice that $C$ is open.

# Union and Intersection

_**(corollary, from [[Open Set#Union and Intersection|this theorem]])**_

If $A$ and $B$ are closed, then $A \cup B$ and $A \cap B$ are also closed.

# Using the Limit Points of a Sequence

_**(lemma, from the definition of a [[Limit Point|limit point]])**_ ^3e2221

Let $A \subseteq \mathbb{R}^{n}$.

$A$ is [[Closed Set|closed]] if $\forall \text{ convergent } \{ a_{k} \} \subseteq A$ (a [[Sequence|sequence]]), the limit point of $a_k$ is in $A$.
