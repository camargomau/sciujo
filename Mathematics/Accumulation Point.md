---
date: 2022-08-24
type: 🧠
tags:
  - MAC/3/C3
---

**Topics:** [[Calculus]] - [[Topology]]

---

_**(definition)**_

Let $A \subseteq \mathbb{R}^{n}$ and $x \in \mathbb{R}^{n}$. We say that $x$ is an _accumulation point_ of $A$ if $\forall r > 0$:

$$
(B_{r}(x) - \{x\}) \cap A \neq \varnothing
$$

_**(observation)**_

$x \in \text{int}(A) \implies x \text{ is an accumulation point}$

> [!example]-
>
> Let $A = (0, 1) \subseteq \mathbb{R}$.
>
> In this case, the accumulation points are $[0,1]$ (the interior points of $A$ and its [[Boundary Point|boundary points]]).
>
> > [!abstract]- Proof for $0$
> > Let $r > 0$, then we have that:
> >
> > $$B_{r}(0) - \{0\} \cap (0,1) \neq \varnothing$$
> >
> > …since $\frac{r}{2} \in B_{r}(0), \frac{r}{2} \in A, \frac{r}{2} \neq 0$.
>
> > [!abstract]- Proof for $1$
> > Let $r>0$, then we have that:
> >
> > $$B_{r}(1) - \{1\} \cap (0,1) \neq \varnothing$$
> >
> > …since $1 - \frac{r}{2} \in B_{r}(1), 1 - \frac{r}{2} \in (0,1)$ (note that $| 1 - \frac{r}{2} - 1 | = \frac{r}{2}$).
>
> Also note that any point in $[0,1]^{c}$ (the [[Complement Set|complement set]]) isn't an accumulation point.
>
> > [!abstract]- Proof
> > $[0,1]^{c}$ is closed, since:
> >
> > $$[0,1]^{c} = (\infty, 0) \cup (1, \infty)$$
> >
> > Then, if $x \in [0, 1]^{c} \implies \exists\ r > 0$ such that:
> >
> > $$B_{r}(x) \subseteq [0,1]^{c}$$
> >
> > Therefore, we have that $B_{r}(x) \cap (0,1) = \varnothing$.
