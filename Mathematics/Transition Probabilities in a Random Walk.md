---
date: 2024-04-03
type: 🧠
---

**Topics:** [[Random Walk]]

---

_**(theorem)**_

Let $\left\{ X_{n} \mid n \in \mathbb{N} \right\}$ be a [[Random Walk|random walk]]. 

For any two integers $x$ and $k$, either **both** even or **both** odd, such that $-n \leq x \leq n$, we have:

- …when $X_{0} = 0$ (it's a simple random walk):

$$
\mathbb{P}\left( X_{n} = x \mid X_{0} = 0 \right) = \binom{n}{\frac{1}{2} (n+x)} \ p^{\frac{1}{2} (n+x)} q^{\frac{1}{2} (n-x)} 
$$

- …when $X_{0} = y \neq 0$, then:

$$
\mathbb{P}\left( X_{n} = x \mid X_{0} = y \right) = \binom{n}{\frac{1}{2} (n+x-y)} \ p^{\frac{1}{2} (n+x-y)} q^{\frac{1}{2} (n-x+y)} 
$$
