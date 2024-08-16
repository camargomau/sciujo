---
date: 2023-09-22
type: 🧠
tags:
  - MAC/5/E1
---

**Topics:** [[Statistics]] - [[Probability]] - [[Random Sample]]

---

_**(theorem)**_

Let $X_{1}, \dots, X_{n}$ be a [[Random Sample|random sample]] such that $\mathbb{E}[X{_{i}}] = \mu$ y $\mathrm{Var}(X_{i}) = \sigma^{2}$ for every $X_{i}$.

Concerning the [[Sampling Distribution|sampling distribution]] of the [[Mean|mean]] $\overline{X}$ of our random sample, then:

$$
\begin{align*}
\mathbb{E}\left[ \overline{X} \right] &= \mu \\
\mathrm{Var}\left( \overline{X} \right) &= \frac{\sigma^{2}}{n}
\end{align*}
$$

> [!quote]- Proof
> See that for the [[Expected Value|expected value]]:
>
> $$
> \begin{align*}
> \mathbb{E}\left[ \overline{X} \right] &= \mathbb{E}\left[ \frac{1}{n} \sum_{i=1}^{n} X_{i} \right] \\
> &= \mathbb{E}\left[ \frac{1}{n} (X_{1} + \dots + X_{n}) \right] \\
> &= \frac{1}{n} \left( \mathbb{E}[X_{1}] + \dots + \mathbb{E}[X_{n}] \right) \\
> &= \frac{1}{n} (\mu + \dots + \mu) \\
> &= \frac{n \mu}{n} \\
> &= \mu
> \end{align*}
> $$
>
> As for the [[Variance|variance]]:
>
> $$
> \begin{align*}
> \mathrm{Var}\left( \overline{X} \right) &= \mathrm{Var}\left( \frac{1}{n} \sum_{i=1}^{n} X_{i} \right) \\
> &= \mathrm{Var}\left( \frac{1}{n} [X_{1} + \dots + X_{n}] \right) \\
> &= \frac{1}{n^{2}} \left[ \mathrm{Var}(X_{1}) + \dots + \mathrm{Var}(X_{n}) \right] \\
> &= \frac{1}{n^{2}} [\sigma^{2} + \dots + \sigma^{2}] \\
> &= \frac{n \sigma^{2}}{n^{2}} \\
> &= \frac{\sigma^{2}}{n}
> \end{align*}
> $$
