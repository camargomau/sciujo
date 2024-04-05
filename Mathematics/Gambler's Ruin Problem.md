---
date: 2024-04-03
type: 🧠
tags:
  - MAC/6/PE
---

**Topics:** [[Random Walk]] - [[Stochastic Process]]

---

Say we're studying a game between two players A and B. In it, there's a probability $p$ of winning and $q$ of losing; there can't be a draw.

The two players agree on giving each other a monetary unit upon losing. Player A starts with $K$ units, while B starts with $N-K$, adding up to a total of $N$. 

_**(theorem)**_

Let $\left\{ X_{n} \mid n \in \mathbb{N} \right\}$ be the [[Stochastic Process|stochastic process]] that represents the wealth of player A at the time $n$. 

This stochastic process is a [[Random Walk|random walk]] that starts at $K$ and finishes either at $0$ (player A is ruined) or at $N$ (player B is ruined). Hence, $0$ and $N$ are both [[Absorbing Set|absorbing states]].

We can obtain the [[Probability of Ruin in the Gambler's Ruin Problem|probability of ruin of a given player]], as well as the [[Expected Amount of Bets Before Ruin in the Gambler's Ruin Problem|expected amount of bets before a given player gets ruined]].