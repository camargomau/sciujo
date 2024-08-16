---
date: 2022-08-25
type: 🧠
tags:
  - MAC/3/MN1
---

**Topics:** [[Numerical Analysis]] - [[Error]]

---

Let $p$ and $q$ be two exact values, and $\hat p$ and $\hat q$, their respective approximate values; $\hat p$ and $\hat q$ have the [[Error|errors]] $\varepsilon_{p}$ and $\varepsilon_q$.

That is:

$$
p = \hat p + \varepsilon_{p}
$$

$$
q = \hat q + \varepsilon_{q}
$$

# Effect on Addition and Subtraction

The effect of the errors on addition and subtraction is:

$$
p \pm q = (\hat p + \varepsilon_{p}) \pm (\hat q + \varepsilon_{q}) = (\hat p \pm \hat q) + (\varepsilon_{p} + \varepsilon_{q})
$$

Notice that, effectively, the errors are **added** when _both_ adding and subtracting $p$ and $q$ with their approximate values.

# Effect on Product and Division

In the case of the product, we have that:

$$
pq = (\hat p + \varepsilon_{p})(\hat q + \varepsilon_{q}) = \hat p \hat q + \hat p \varepsilon_{q} + \hat q \varepsilon_{p} + \varepsilon_{p} \varepsilon_{q}
$$

If the approximate values $\hat p$ and $\hat q$ are greater that $1$, then the error will grow in a significative way.

Given $p \neq 0$ and $\hat p, \hat q$ good approximations, we can show that the [[Relative Error|relative error]] of the product of two numbers is approximately the sum of the relative errors of the individual approximations:

$$
E_{r_{pq}} = \frac{pq - \hat p \hat q}{pq} \approx \frac{\varepsilon_{p}}{p} + \frac{\varepsilon_{q}}{q} + 0 = E_{r_{p}} + E_{r_{p}}
$$
