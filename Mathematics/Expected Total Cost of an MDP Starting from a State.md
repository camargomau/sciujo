---
date: 2024-05-18
type: 🧠
tags:
  - MAC/6/PE
---

**Topics:** [[Policy Improvement Method for MDPs]] - [[Markov Decision Process]]

---

_**(definition)**_

In the context of an [[Markov Decision Process|MDP]], let $V_{i}^n\{r\}$ be the **[[Expected Value|expected]] total cost of a system that starts in [[State Set|state]] $i$ and evolves over $n$ periods**, given a specific [[Markov Decision Process Policy|policy]] $r$. This will be:

$$
V_{i}^{n}\{k\} = C_{ik} + \alpha \sum_{j=0}^{m} p_{ij}\{k\} \ V_{j}^{n-1}\{r\}
$$

…where $C_{ik}$ is the cost of making the decision $k$ in the state $i$ (as defined by the policy $r$) and $\alpha$ is the discount factor. If there is no discount, then $\alpha = 1$, as is the case when using the standard [[Policy Improvement Method for MDPs|policy improvement method]] (cf. the [[Discounted Policy Improvement Method for MDPs|discounted version]]).

> [!tip]- Explanation
> Notice that this sum is basically the sum of:
> - $C_{ik}$, the cost of the first period, when the system goes from $i$ to another state $j$.
> - $\sum_{j=0}^{m} p_{ij}\{k\} \ V_{j}^{n-1}\{r\}$, the weighted sum of the total costs that could be incurred by continuing from another state $j$ (and still following the same policy $r$).

**Do not forget** that these calculations take into consideration a given **policy $r$**, which defines which decision $k$ is made in which state $i$.
