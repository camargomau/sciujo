---
date: 2024-05-18
type: 🧠
tags:
  - MAC/5/PE
---

**Topics:** [[Markov Decision Process]] - [[Optimisation]]

---

There are several [[Optimisation|optimisation]] methods that allow us to find the optimal [[Markov Decision Process Policy|policy]] for a given [[Markov Decision Process|Markov decision process]]:

- The [[Exhaustive Enumeration Method for MDPs|exhaustive enumeration method]] is the simplest of them all. It consists of enumeration all of the viable policies, calculating the expected cost for each one, then finally selecting the optimal one. It's simple but computationally expensive.

- Solving the [[MDP as a Linear Programming Problem|MDP as a linear programming problem]] through any of the applicable methods. 

- The [[Policy Improvement Method for MDPs|policy improvement method]] consists of solving a linear equation system, then finding an alternative policy that optimises the costs until the optimal policy is reached. Compared to other methods, it is rather efficient and simple.

	- The [[Discounted Policy Improvement Method for MDPs|discounted policy improvement method]] is basically the same method applied for phenomena where it might prove useful to discount the costs the further they are in the future. 

- The [[Successive Approximations Method for MDPs|successive approximations method]] finds an _approximation_ to the optimal policy by using the expected total costs starting from every state given $n$ increasing remaining periods. 