---
date: 2023-03-25
type: 🧠
tags:
  - MAC/4/MN2
---

**Topics:** [[Interpolation]]

---

Let $y = f(x)$ be a [[Function|function]] whose exact definition we don't know. All we know is various values of $f(x)$, like so:

| $\mathbf{x_i}$ | $\mathbf{y_i =  f(x_i)}$ |
|:--------------:|:------------------------:|
|     $x_0$      |          $y_0$           |
|     $x_1$      |          $y_1$           |
|     $x_2$      |          $y_2$           |
|     $x_3$      |          $y_3$           |
|    $\vdots$    |         $\vdots$         |
|     $x_n$      |          $y_n$           |

Just like the tables we use for [[Newton's Divided Differences Interpolation Method|Newton's divided differences method]], and unlike the ones used for [[Newton's Finite Differences Interpolation Method|Newton's finite differences method]], the spacing between every $x_i$ does **not** need to be constant.

We will be able to interpolate $y_k = f(x_k)$ for any $x_k$ within the constraints of the table by using a method known as _Hermite's interpolation method_.

# $z_i$

Just like Newton's divided and finite differences method, we will use a table to aid us. This time around, though, instead of using $x_i$ as the main "measure", we will use $z_i$.

For every $i = 0, 1, \dots, n$, let $z_{2i}$ be:

$$
z_{2i} = z_{2i+1} = x_i
$$

> [!example]- In a Table
> More simply, in a table:
>
> | $\mathbf{z_i}$   | $\mathbf{f(z_i)}$      |
> | ---------------- | ---------------------- |
> | $z_0 = x_0$      | $f(z_0) = f(x_0)$      |
> | $z_1 = x_0$      | $f(z_1) = f(x_0)$      |
> | $z_2 = x_1$      | $f(z_2) = f(x_1)$      |
> | $z_3 = x_1$      | $f(z_3) = f(x_1)$      |
> | $z_4 = x_2$      | $f(z_4) = f(x_2)$      |
> | $z_5 = x_2$      | $f(z_5) = f(x_2)$      |
> | $\vdots$         | $\vdots$               |
> | $\vdots$         | $\vdots$               |
> | $z_{2n} = x_n$   | $f(z_{2n}) = f(x_n)$   |
> | $z_{2n+1} = x_n$ | $f(z_{2n+1}) = f(x_n)$ |

# Differences

We'll also use differences, just like Newton's [[Newton's Finite Differences Interpolation Method|finite]] and [[Newton's Divided Differences Interpolation Method|divided differences]] methods.

In fact, most of the differences will be just like the ones used in Newton's divided differences method.

The only exceptions will be in the _even-numbered first differences_ (if we start counting from $0$):

$$
\begin{align*}
f[z_0, z_1] &= f'(x_0) \\
f[z_2, z_3] &= f'(x_1) \\
f[z_4, z_5] &= f'(x_2) \\
\vdots \\
f[z_{2i}, z_{2i+1}] &= f'(x_i) \\
\end{align*}
$$

> [!question]- How to find the derivative?
> Let's say we're calculating all of these differences from scratch. If we don't know the function yet, how can we derivate it?
>
> Easy. We obtain an approximating polynomial first by using one of the many other [[Interpolation|interpolation]] methods we know, then we derivate it.

The rest are the familiar divided differences. For rest of the _first differences_:

$$
\begin{align*}
f[z_1, z_2] &= \frac{f(z_2) - f(z_1)}{z_2 - z_1} \\
f[z_3, z_4] &= \frac{f(z_4) - f(z_3)}{z_4 - z_3} \\
\vdots \\
f[z_i, z_{i+1}] &= \frac{f(z_{i+1}) - f(z_i)}{z_{i+1} - z_i} \\
\end{align*}
$$

In general, for the $n$th difference:

$$
f[z_i, z_{i+1}, z_{i+2}, \dots, z_{i+n}] = \frac{f[z_{i+1}, z_{i+2}, \dots, z_{i+n}] - f[z_i, z_{i+1}, \dots, z_{i+n-1}]}{z_{i+n} - z_i}
$$

> [!example]- Differences Table
> Similarly to Newton's finite and divided differences method, we can build a differences table to better visualise all these differences:
>
> |  $\mathbf{z_i}$  |   $\mathbf{f(z_i})$    |            $\mathbf{f[z_i, z_{i+1}]}$             | $\mathbf{f[z_i, z_{i+1}, z_{i+2}]}$ | $\mathbf{f[z_i, z_{i+1}, z_{i+2}, z_{i+3}]}$ |
> |:----------------:|:----------------------:|:-------------------------------------------------:|:-----------------------------------:|:--------------------------------------------:|
> |   $z_0 = x_0$    |   $f(z_0) = f(x_0)$    |                                                   |                                     |                                              |
> |                  |                        |              $f[z_0, z_1] = f'(x_0)$              |                                     |                                              |
> |   $z_1 = z_0$    |   $f(z_1) = f(z_0)$    |                                                   |         $f[z_0, z_1, z_2]$          |                                              |
> |                  |                        | $f[z_1, z_2] = \frac{f(z_2) - f(z_1)}{z_2 - z_1}$ |                                     |           $f[z_0, z_1, z_2, z_3]$            |
> |   $z_2 = z_1$    |   $f(z_2) = f(z_1)$    |                                                   |         $f[z_1, z_2, z_3]$          |                                              |
> |                  |                        |              $f[z_2, z_3] = f'(x_1)$              |                                     |           $f[z_1, z_2, z_3, z_4]$            |
> |   $z_3 = z_1$    |   $f(z_3) = f(z_2)$    |                                                   |         $f[z_2, z_3, z_4]$          |                                              |
> |                  |                        | $f[z_3, z_4] = \frac{f(z_4) - f(z_3)}{z_4 - z_3}$ |                                     |           $f[z_2, z_3, z_4, z_5]$            |
> |     $\vdots$     |        $\vdots$        |                     $\vdots$                      |              $\vdots$               |                   $\vdots$                   |
> |     $\vdots$     |        $\vdots$        |                     $\vdots$                      |              $\vdots$               |                   $\vdots$                   |
> |     $\vdots$     |        $\vdots$        |                     $\vdots$                      |              $\vdots$               |  $f[z_{2n-2}, z_{2n-1}, z_{2n}, z_{2n+1}]$   |
> |  $z_{2n} = z_n$  |  $f(z_{2n}) = f(z_n)$  |                     $\vdots$                      |   $f[z_{2n-1}, z_{2n}, z_{2n+1}]$   |                                              |
> |                  |                        |          $f[z_{2n}, z_{2n+1}] = f'(x_n)$          |                                     |                                              |
> | $z_{2n+1} = x_n$ | $f(z_{2n+1}) = f(x_n)$ |                                                   |                                     |                                              |

# Interpolation Formula

Given an $x_k$ contained within the constraints of the table (i.e. $x_0 \leq x_k \leq x_n$), we can use these differences to [[Interpolation|interpolate]] its $f(x_k) = H_{2n+1}(x_k)$ with the following formula that is used to obtain an _interpolating polynomial_.

We'll choose a specific $z_i$ in our table as an anchor value; we'll set this value to be $z_0$.

$$
\begin{align*}\\
H_{2n+1} (x_k) = &\ f(z_0) + (x_k - z_0) f[z_0, z_1] + (x_k - z_1)(x_k - z_0) f[z_0, z_1, z_2] \\
&+ (x_k - z_2)(x_k - z_1)(x_k - z_0) f[z_0, z_1, z_2, z_3] + \dots \\
&+ (x_k - z_{k-1}) \dots (x_k - z_0) + [z_0, \dots, z_k]
\end{align*}
$$

Indeed, this formula is equivalent to Newton's [[Newton's Finite Differences Interpolation Method|finite]] and [[Newton's Divided Differences Interpolation Method|divided differences]]' forwards interpolation formulas. We can come up with a backwards interpolation formula for Hermite's method, but notice we can just flip our table upside down and then interpolate with this formula to get the same result.
