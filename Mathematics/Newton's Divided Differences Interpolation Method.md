---
date: 2023-03-25
type: 🧠
tags:
  - MAC/S4/MN2
---

**Topics:** [[Interpolation]]

---

Let $y = f(x)$ be a [[Function|function]] whose exact definition we don't know. All we know is various values of $f(x)$, like so:

| $\mathbf{x_i}$ | $\mathbf{f(x_i)}$ |
|:--------------:|:-----------------:|
|     $x_0$      |      $f(x_0)$      |
|     $x_1$      |      $f(x_1)$      |
|     $x_2$      |      $f(x_2)$      |
|     $x_3$      |      $f(x_3)$      |
|    $\vdots$    |     $\vdots$      |
|     $x_n$      |      $f(x_n)$      |

Unlike the tables we use for [[Newton's Finite Differences Interpolation Method|Newton's finite differences method]], the spacing between every $x_i$ does **not** need to be constant.

We will be able to interpolate $f(x_k)$ for any $x_k$ within the constraints of the table by using a method known as _Newton's finite divided interpolation method_.

# Differences

Just like Newton's finite differences method, Newton's divided differences method uses, well, differences.

For this method, the _first differences_ are as follows:

$$
\begin{align*}
f[x_0, x_1] &= \frac{f(x_1) - f(x_0)}{x_1 - x_0} \\
f[x_1, x_2] &= \frac{f(x_2) - f(x_1)}{x_2 - x_1} \\
\vdots \\
f[x_i, x_{i+1}] &= \frac{f(x_{i+1}) - f(x_i)}{x_{i+1} - x_i} \\
\end{align*}
$$

The _second differences_ are:

$$
\begin{align*}
f[x_0, x_1, x_2] &= \frac{f[x_1, x_2] - f[x_0, x_1]}{x_2 - x_0} \\
f[x_1, x_2, x_3] &= \frac{f[x_2, x_3] - f[x_1, x_2]}{x_3 - x_1} \\
\vdots \\
f[x_i, x_{i+1}, x_{i+2}] &= \frac{f[x_{i+1}, x_{i+2}] - f[x_i, x_{i+1}]}{x_{i+2} - x_i}
\end{align*}
$$

In general, the $n$th difference is:

$$
f[x_i, x_{i+1}, x_{i+2}, \dots, x_{i+n}] = \frac{f[x_{i+1}, x_{i+2}, \dots, x_{i+n}] - f[x_i, x_{i+1}, \dots, x_{i+n-1}]}{x_{i+n} - x_i}
$$

Of course, the amount of difference tiers will depend on the amount of points we know.

> [!example]- Differences Table
> With all these differences, we can build a table of differences just like the one we can build with [[Newton's Finite Differences Interpolation Method|Newton's finite differences method]]:
>
> | $\mathbf{x_i}$ | $\mathbf{f(x_i})$ | $\mathbf{f[x_i, x_{i+1}]}$ | $\mathbf{f[x_i, x_{i+1}, x_{i+2}]}$ | $\mathbf{f[x_i, x_{i+1}, x_{i+2}, x_{i+3}]}$ |
> |:--------------:|:-----------------:|:--------------------------:|:-----------------------------------:|:--------------------------------------------:|
> |     $x_0$      |     $f(x_0)$      |                            |                                     |                                              |
> |                |                   |       $f[x_0, x_1]$        |                                     |                                              |
> |     $x_1$      |     $f(x_1)$      |                            |         $f[x_0, x_1, x_2]$          |                                              |
> |                |                   |       $f[x_1, x_2]$        |                                     |           $f[x_0, x_1, x_2, x_3]$            |
> |     $x_2$      |     $f(x_2)$      |                            |         $f[x_1, x_2, x_3]$          |                                              |
> |                |                   |       $f[x_2, x_3]$        |                                     |           $f[x_1, x_2, x_3, x_4]$            |
> |     $x_3$      |     $f(x_3)$      |                            |         $f[x_2, x_3, x_4]$          |                                              |
> |                |                   |       $f[x_3, x_4]$        |                                     |           $f[x_2, x_3, x_4, x_5]$            |
> |    $\vdots$    |     $\vdots$      |          $\vdots$          |              $\vdots$               |                   $\vdots$                   |
> |    $\vdots$    |     $\vdots$      |          $\vdots$          |              $\vdots$               |                   $\vdots$                   |
> |    $\vdots$    |     $\vdots$      |          $\vdots$          |              $\vdots$               |     $f[x_{n-3}, x_{n-2}, x_{n-1}, x_n]$      |
> |   $x_{n-1}$    |   $f(x_{n-1})$    |          $\vdots$          |     $f[x_{n-2}, x_{n-1}, x_n]$      |                                              |
> |                |                   |     $f[x_{n-1}, x_n]$      |                                     |                                              |
> |     $x_n$      |     $f(x_n)$      |                            |                                     |                                              |

# Interpolation Formulas

Given an $x_k$ contained within the constraints of the table (i.e. $x_0 \leq x_k \leq x_n$), we can use these differences to [[Interpolation|interpolate]] its $f(x_k)$ with one of two formulas that are used to obtain an _interpolating polynomial_.

For both of them, we choose a specific $x_i$ in our table as an anchor value; we'll set this value to be $x_0$.

Our choice between these two formulas will depend on the amount of differences that can be used with a given one (the greater, the better the approximation), as well as on how close $x_k$ is to $x_0$ (the closer, the better).

## Forwards Interpolation

We can obtain an approximation to our $y_k = f(x_k)$ with the _forwards interpolation_ formula:

$$
\begin{align*}
f(x_k) =\ &f(x_0) + (x_k - x_0) f[x_0, x_1] \\
&+ (x_k - x_1)(x_k - x_0) f[x_0, x_1, x_2] \\
&+ \dots \\
&+ (x_k - x_{k-1})(x_k - x_{k-2})\dots(x_k - x_0) f[x_0, x_1, \dots, x_k]
\end{align*}
$$

## Backwards Interpolation

We can also obtain our $y_k = f(x_k)$ with the _backwards interpolation_ formula:

$$
\begin{align*}
f(x_k) =\ &f(x_n) + (x_k - x_n) f[x_{n-1}, x_n] \\
&+ (x_k - x_n)(x_k - x_{n-1}) f[x_{n-2}, x_{n-1}, x_n] \\
&+ \dots \\
&+ (x_k - x_n)\dots(x_k - x_{k+1}) f[x_k, x_{k-1}, \dots, x_n]
\end{align*}
$$
