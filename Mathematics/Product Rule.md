---
date: 2023-02-20
type: 🧠
tags:
  - MAC/4/PB
---

**Topics:** [[Probability]]

---

_**(definition)**_

Let $A_1, \dots, A_n \in \mathscr{F}$ (a [[σ-Algebra|sigma-algebra]]) such that $\mathbb{P}(A_1 \cap \dots \cap A_{n-1}) > 0$.

Then, the probability of the intersection of all these sets is:

$$
\begin{align*}
\mathbb{P}(A_1 \cap A_2 \cap \dots \cap A_n) :=\ &\mathbb{P}(A_n \mid A_1 \cap A_2 \cap \dots \cap A_{n-1}) \\
& \mathbb{P}(A_{n-1} \mid A_1 \cap \dots \cap A_{n-2}) \\
& \dots \\
& \mathbb{P}(A_3 \mid A_1 \cap A_2) \\
& \mathbb{P}(A_2 \mid A_1) \\
& \mathbb{P}(A_1)
\end{align*}
$$

(see [[Conditional Probability|conditional probability]])
