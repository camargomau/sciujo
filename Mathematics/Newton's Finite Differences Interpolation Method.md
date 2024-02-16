---
date: 2023-03-10
type: 🧠
tags:
  - MAC/S4/MN2
---

**Topics:** [[Interpolation]]

---

Let $y = f(x)$ be a [[Function|function]] whose exact definition we don't know. All we know is various values of $f(x)$, like so:

|  $\mathbf{x_i}$  | $\mathbf{y_i =  f(x_i)}$ |
|:----------------:|:------------------------:|
|      $x_0$       |          $y_0$           |
| $x_1 = x_0 + h$  |          $y_1$           |
| $x_2 = x_0 + 2h$ |          $y_2$           |
| $x_3 = x_0 + 3h$ |          $y_3$           |
|     $\vdots$     |         $\vdots$         |
| $x_n = x_0 + nh$ |          $y_n$           |

Notice that every $x_i$ **must** be spaced by a **constant** $h$, so that $x_k = x_0 + kh$.

> [!tip]- Non-Constant Spacing
> If we have a table where the spacing between every $x_i$ is not constant, then we must use another interpolation method, like [[Newton's Divided Differences Interpolation Method|Newton's divided differences method]], which is very similar to this one.

We will be able to interpolate $y_k = f(x_k)$ for any $x_k$ within the constraints of the table by using a method known as _Newton's finite differences interpolation method_.

# Differences

First, we'll define what a difference is.

The _first differences_ are the differences between two consecutive values of $y$. We denote these differences as $a_i$:

$$
\begin{align*}
a_0 &= y_1 - y_0 \\
a_1 &= y_2 - y_1 \\
a_2 &= y_3 - y_2 \\
\vdots \\
a_k &= y_{k+1} - y_k \\
\end{align*}
$$

Similarly, the _second differences_ are the differences between two consecutive first differences, and they are denoted as $b_i$:

$$
\begin{align*}
b_0 &= a_1 - a_0 \\
b_1 &= a_2 - a_1 \\
b_2 &= a_3 - a_2 \\
\vdots \\
b_k &= a_{k+1} - a_k \\
\end{align*}
$$

In the same way, we have third differences $c_i$, fourth differences $d_i$, etc. We can also write these differences as $\Delta y_i$, $\Delta^2 y_i$, $\Delta^3 y_i$, etc.

The number of difference tiers we have will depend on the size of our table (the amount of known points).

> [!example]- Differences Table
> We can arrange all these differences in a table like so:
>
> | $\mathbf{x_i}$ | $\mathbf{y_i}$ | $\mathbf{a_i}$ | $\mathbf{b_i}$ | $\mathbf{c_i}$ | $\mathbf{d_i}$ |
> |:--------------:|:--------------:|:--------------:|:--------------:|:--------------:|:--------------:|
> |     $x_0$      |     $y_0$      |                |                |                |                |
> |                |                |     $a_0$      |                |                |                |
> |     $x_1$      |     $y_1$      |                |     $b_0$      |                |                |
> |                |                |     $a_1$      |                |     $c_0$      |                |
> |     $x_2$      |     $y_2$      |                |     $b_1$      |                |     $d_0$      |
> |                |                |     $a_2$      |                |     $c_1$      |                |
> |     $x_3$      |     $y_3$      |                |     $b_2$      |                |     $d_1$      |
> |                |                |     $a_3$      |                |     $c_2$      |                |
> |    $\vdots$    |    $\vdots$    |    $\vdots$    |    $\vdots$    |    $\vdots$    |    $\vdots$    |
> |    $\vdots$    |    $\vdots$    |    $\vdots$    |    $\vdots$    |    $\vdots$    |   $d_{n-4}$    |
> |    $\vdots$    |    $\vdots$    |    $\vdots$    |    $\vdots$    |   $c_{n-3}$    |                |
> |   $x_{n-1}$    |   $y_{n-1}$    |    $\vdots$    |   $b_{n-2}$    |                |                |
> |                |                |   $a_{n-1}$    |                |                |                |
> |     $x_n$      |     $y_n$      |                |                |                |                |

# Interpolation Formulas

Given an $x_k$ contained within the constraints of the table (i.e. $x_0 \leq x_k \leq x_n$), we can use these differences to [[Interpolation|interpolate]] its $y_k = f(x_k)$ with one of two formulas that are used to obtain an _interpolating polynomial_.

For both of them, we choose a specific $x_i$ in our table as an anchor value; we'll set this value to be $x_0$.

Our choice between these two formulas will depend on the amount of differences that can be used with a given one (the greater, the better the approximation), as well as on how close $x_k$ is to $x_0$ (the closer, the better).

## Forwards Interpolation

Let $k$ be:

$$
k = \frac{x_k - x_0}{h}
$$

We can obtain an approximation to our $y_k = f(x_k)$ with the _forwards interpolation_ formula:

$$
y_k = y_0 + ka_0 + \frac{k(k-1)}{2!}b_0 + \frac{k(k-1)(k-2)}{3!}c_0 + \dots
$$

## Backwards Interpolation

Let $k$ be:

$$
k = \frac{x_0 - x_k}{h}
$$

We can obtain our $y_k = f(x_k)$ with the _backwards interpolation_ formula:

$$
y_{k} = y_0 - ka_{-1} + \frac{k(k-1)}{2!}b_{-2} - \frac{k(k-1)(k-2)}{3!}c_{-3} + \dots
$$
