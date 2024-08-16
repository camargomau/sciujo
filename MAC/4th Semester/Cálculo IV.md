---
type: 🏫
tags:
  - MAC/4/C4
---

# Unit 1: Vector-Valued Functions

A [[Vector-Valued Function|vector-valued function]] (_función de valor vectorial_) is a function that returns vectors instead of points. We graph vector-valued functions by joining the extreme ends of all the vectors it returns.

[[Continuous Vector-Valued Function|Continuity can be defined for vector-valued functions]], and they can also have:

- [[Limit of a Vector-Valued Function|Limits]]
- [[Derivative of a Vector-Valued Function|Derivatives]] (and [[Derivative of Operated Vector-Valued Functions|operated]])
- [[Antiderivative of a Vector-Valued Function|Antiderivatives]] and [[Defined Integral of a Vector-Valued Function|defined integrals]]

## Curves

Given any curve, we can calculate its [[Arc Length|arc length]] by using the derivative of its function and then integrating. We can parametrise a curve such that it is drawn at a speed that corresponds to its arc length; we call such a parametrisation an [[Arc Length Parameter|arc length parametrisation]].

Curves can have [[Tangent Unit Vector|tangent unit vectors]], [[Normal Unit Vector|normal unit vectors]] and [[Binormal Vector|binormal vectors]] at their points.

Curves can be [[Smooth Curve|smooth]]. We can also define the [[Curvature|curvature]] of a curve.

## Physics

Vector-valued functions are especially useful in physics, since they help us describe an object's position, and through their derivatives, its speed and acceleration, among many other physical concepts.

For instance, they help us describe the [[Tangential and Normal Components of Acceleration|tangential and normal components of acceleration]], which can, in turn, help us understand better certain phenomena, like the behaviour of a car on a curve.

# Unit 2: Vector Fields

A [[Vector Field|vector field]] is a function that goes from $\mathbb{R}^n$ to $V_n$ (a vector space of dimension $n$). The graphical representation of a vector fields involves drawing the vectors that the function returns, starting on the coordinates that were given to it.

A [[Potential Function|potential function]] of a vector field is a vector-valued function whose gradient vector is equal to said vector field. A conservative vector field is one that has (one or several) potential functions.

We can obtain the _curl_ and _divergence_ of a given vector field. These two operators help us know the behaviour of the vectors that the vector field returns:

- [[Curl of a Vector Field|Curl]] tells us the rate of rotation of the [[Vector|vectors]] in a vector field.
- [[Divergence of a Vector Field|Divergence]] tells us how much the vectors "grow" or "shrink"

Additionally, the [[Laplacian of a Function|Laplacian]] of a vector-valued function is defined as the divergence of the function's gradient vector.

# Unit 3: Path and Line Integrals

The [[Path Integral|path integral]] (of a **scalar** function over a curve) is a special type of integral that has [[Path Integral Applications|many applications]], such as calculating the area of complex surfaces, calculating the average of a function over a curve, or calculating the centre of mass of an object.

The [[Line Integral|line integral]] (of a **vector field** over a curve) is another special type of integral. In general, it's the equivalent of a path integral, but for vector fields instead of scalar functions. Line integrals also have many applications, such as calculating the work done by moving an object over a curve with a force defined by a vector field.

> [!info]- Naming
> In all my notes, _path integral_ refers to the integral of a **scalar** function over a curve, while _line integrals_ refers to the integral of a **vector field** over a curve.
>
> Some authors call both _line integrals_ (of a scalar field and of a vector field, respectively).

Line integrals help us understand [[Conservative Vector Field|conservative vector fields]] (vector fields that are the gradient of some scalar function) better. The line integral of _any_ conservative vector field over a curve will only depend on the two endpoints of the curve, with no regard for the actual chosen curve. We call this _path independence_.

# Unit 4: Surface Integrals

Similarly to path and line integrals, which are based off of a curve, we can define the [[Integral of a Surface|integral of a surface]] and the [[Integral of a Vector Field over a Surface|integral of a vector field over a surface]].
