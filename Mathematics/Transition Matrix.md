---
date: 2024-04-04
type: 🧠
---

**Topics:** [[Markov Chain]] - [[Transition Probabilities in a Markov Chain]] - [[n Step Transition Probability]]

---

_**(definition)**_

Given a [[Markov Chain|Markov chain]] with $m$ total states, we can handily write its [[n Step Transition Probability|n step transition probabilities]] $p_{ij}^{(n)}$ in a **transition matrix**, which is an $m \times m$ matrix of the form:

$$
P^{(n)} =
\begin{pmatrix}
p_{00}^{(n)} & p_{01}^{(n)} & \dots & p_{0m}^{(n)} \\
p_{10}^{(n)} & p_{11}^{(n)} & \dots & p_{1m}^{(n)} \\
\vdots & \vdots & \ddots & \vdots \\
p_{m0}^{(n)} & p_{m1}^{(n)} & \dots & p_{mm}^{(n)} \\
\end{pmatrix}
$$

That is, the $ij$th element of the transition matrix is the transition probability from $i$ to $j$ in $n$ steps.

# $n$ step Transition Matrix

_**(theorem)**_

From the [[Chapman-Kolmogorov Equation|Chapman-Kolmogorov equation]] it follows that:

$$
P^{(n)} = \left( P^{(1)} \right)^{n}
$$

That is, [[Matrix Exponentiation|matrix exponentiation]].
