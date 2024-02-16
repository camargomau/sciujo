---
date: 2023-02-11
type: 🧠
tags:
  - MAC/S4/PB
---

**Topics:** [[Probability Measure]] - [[Probability]]

---

_**(theorem)**_

Let $\mathbb{P}(A)$ be the [[Probability Measure|probability measure]] of an [[Event|event]] $A$. This probability measure has the following properties:

1. $\mathbb{P}(A^c) = 1 - \mathbb{P}(A)$
2. $\mathbb{P}(\varnothing) = 0$
3. If $A \subset B$, then $\mathbb{P}(B \backslash A) = \mathbb{P}(B) - \mathbb{P}(A)$
4. The probability measure is [[Monotonic|monotonic]]. That is:

$$
A \subset B \implies \mathbb{P}(A) \leq \mathbb{P}(B)
$$

# Finite Additivity

_**(theorem)**_

Let $A_1, \dots, A_n \in \mathscr{F}$, where $A_i \cap A_j = \varnothing$ ($i \neq j$; [[Disjoint Set|disjoint]]). Then:

$$
\mathbb{P}\left( \cup_{k=1}^n A_k \right) = \sum_{k=1}^n \mathbb{P}(A_k)
$$

# Finite Subadditivity

_**(theorem)**_

Let $A_1, \dots, A_n \in \mathscr{F}$ not necessarily [[Disjoint Set|disjoint]]. Then:

$$
\mathbb{P}\left( \cup_{k=1}^n A_k \right) \leq \sum_{k=1}^n \mathbb{P}(A_k)
$$

This property is also known as Boole's inequality.

# Inclusion-Exclusion Rule

_**(theorem)**_

Let $A_1, \dots, A_n \in \mathscr{F}$ not necessarily [[Disjoint Set|disjoint]]. Then:

$$
\begin{align}
\mathbb{P} \left( \cup_{k=1}^n A_k \right) =& \sum_{k=1}^n \mathbb{P}(A_k) - \sum_{\substack{i,j=1 \\ i \neq j}}^n \mathbb{P}(A_i \cap A_j) \\
&+ \sum_{\substack{i,j,k=1 \\ i \neq j \neq k}}^n \mathbb{P}(A_i \cap A_j \cap A_k) + \dots \\
&+ (-1)^{n+1} \mathbb{P}(A_i \cap \dots \cap A_n)
\end{align}
$$

> [!todo]- Few events
> Given only two events:
>
> $$
> \mathbb{P}(A \cup B) = \mathbb{P}(A) + \mathbb{P}(B) - \mathbb{P}(A \cap B)
> $$
>
> Given only three events:
>
> $$
> \begin{align} \mathbb{P}(A \cup B \cup C) =&\  \mathbb{P}(A) + \mathbb{P}(B) + \mathbb{P}(C) \\ &- \mathbb{P}(A \cap B) - \mathbb{P}(B \cap C) - \mathbb{P}(A \cap C) \\ &+ \mathbb{P}(A \cap B \cap C) \end{align}
> $$
