---
date: 2023-11-12
type: 🧠
tags:
  - MAC/5/E1
---

**Topics:** [[Estimator]] - [[Statistics]]

---

When trying to obtain [[Estimator|point estimators]], we can use the _moments method_, which consists of (1) equating [[Population|population]] [[Moment|moments]] with their corresponding [[Sample|sample]] moments, and then (2) solving the resulting equation(s).

# Procedure

Let $X$ be a [[Random Variable|random variable]] whose [[Probability Distribution|probability distribution]] is characterised by a [[Parameter (Statistics)|parameter]] that we want to estimate. To find an estimator for this parameter, we can use the moments method, which consists of solving:

$$
\begin{align*}
\mathbb{E}[X] &\simeq \frac{1}{n} \sum_{i=1}^{n} x_{i} = \overline{X} \\
\mathbb{E}[X^{2}] &\simeq \frac{1}{n} \sum_{i=1}^{n} x_{i}^{2} \\
&\vdots \\
\mathbb{E}[X^{n}] &\simeq \frac{1}{n} \sum_{i=1}^{n} x_{i}^{n} \\
\end{align*}
$$

## Continuous Random Variable

If $X$ is a [[Absolutely Continuous Random Variable|continuous random variable]], then, for every relevant $j$, we're just solving:

$$
\mathbb{E}[X^j] = \int_{-\infty}^{\infty} x^j f(x) \ dx 
$$

# Example

Let $X$ be a random variable with [[Density Function|density function]]:

$$
f(x) =
\begin{cases}
\theta x^{\theta-1} & \text{if } 0 \leq x \leq 1 \\
0 & \text{otherwise}
\end{cases}
$$

Notice that it depends on a [[Parameter (Statistics)|parameter]] $\theta$. We can use the moments method to find an estimator $\hat{\theta}$ for $\theta$. We begin by finding $X$'s first sample moment (its [[Expected Value|expected value]]):

$$
\begin{align*}
\mathbb{E}[X] &= \int_{-\infty}^{\infty} x f(x) \ dx \\
&= \int_{0}^{1} x \theta x^{\theta - 1} \ dx  \\
&= \int_{0}^{1} \theta x^{\theta} \ dx \\
&= \left. \left( \frac{\theta}{\theta + 1} x^{\theta + 1} \right) \right|_{0}^{1} \\
&= \frac{\theta}{\theta+1}
\end{align*}
$$

Now, we equate it to $X$'s first population moment (its [[Mean|mean]]). At this point, we are now working with $\hat{\theta}$, the estimator:

$$
\begin{align*}
\frac{\hat{\theta}}{\hat{\theta} + 1} &= \overline{X} \\
\hat{\theta} &= \overline{X} (\hat{\theta} + 1) \\
\hat{\theta} &= \overline{X} \hat{\theta} + \overline{X} \\
\hat{\theta} - \overline{X} \hat{\theta} &= \overline{X} \\
\hat{\theta} (1 - \overline{X}) &= \overline{X} \\
\hat{\theta} &= \frac{\overline{X}}{1 - \overline{X}}
\end{align*}
$$

That's all. We have found that $\hat{\theta} = \left( \frac{\overline{X}}{1-\overline{X}} \right)$ is an estimator for $\theta$, the parameter that $X$'s [[Probability Distribution|distribution]] depends on. 
