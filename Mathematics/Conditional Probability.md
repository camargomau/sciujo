---
date: 2023-02-15
type: 🧠
tags:
  - MAC/4/PB
---

**Topics:** [[Probability]]

---

If we add additional information to an [[Experiment|experiment]], we change the [[Probability of an Event|probability of the event]].

_**(definition)**_

Let $A, B$ be [[Event|events]] such that $\mathbb{P}(B) > 0$.

We define the _conditional probability_ of the event $A$, **given** (i.e. knowing, supposing, assuming) the occurrence of the event $B$, as follows:

$$
\mathbb{P}(A \mid B) := \frac{\mathbb{P}(A \cap B)}{\mathbb{P}(B)}
$$

$\mathbb{P}(A \mid B)$ is read "the probability of $A$ given $B$".

> [!example]-
> Let's throw a die twice.
>
> What's the probability of obtaining a $6$ in one of the throws, **given** different numbers in both throws? This is a conditional probability.
>
> Let:
>
> - $A:$ get a $6$
> - $B:$ get different numbers in both throws
>
> First, note that $B = \{(x,y) \mid x, y \in \{1, \dots, 6 \}, x \neq y \}$ ($|B| = 30$). Thus:
>
> $$
> \mathbb{P}(B) = \frac{|B|}{|\Omega|} = \frac{30}{36}
> $$
>
> On the other hand, $A = \{ (i, 6), (6, j), (6, 6) \mid i, j \in \{1, \dots, 5\} \}$. Thus:
>
> $$
> A \cap B = \{ (i, 6), (6, j) \mid i,j \in \{1, \dots, 5\} \}
> $$
>
> $$
> \implies \mathbb{P}(A \cap B) = \frac{|A \cap B|}{|\Omega|} = \frac{10}{36}
> $$
>
> Finally, with the formula for a conditional probability, we have that:
>
> $$
> \mathbb{P}(A \mid B) = \frac{\frac{10}{36}}{\frac{30}{36}} = \frac{10}{30}= \frac{1}{3}
> $$

_**(theorem)**_

Conditional probability is a [[Probability Measure|probability measure]].
