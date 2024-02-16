---
type: 🏫
tags:
  - MAC/S4/PB
---

# Unit 1: Events and Probability

## Experiments, Sample Spaces and Events

A [[Experiment|random experiment]], denoted $\varepsilon$, is something we do that has various results and can't be predicted.

A [[Sample Space|sample space]], denoted $\Omega$, is the set that contains all the possible results of an experiment. Sample spaces are called _espacios muestrales_ in Spanish.

An [[Event|event]], denoted by any uppercase letter of the Latin alphabet, is a subset of a sample space.

## Frequency and Probability

We can define the [[Frequency|frequency]] and the [[Probability of an Event|probability]] of a given event. The latter is of special importance in probability, as the name suggests.

> [!info]- Frequency vs. Probability
> Note that these two concepts, while they may initially seem the same, are different. Frequency relates the number of times that the event occurs to the number of times **the experiment was carried out**; probability relates the number of times that the event occurs to the number of **total possible cases**.

## σ-algebras and Probability Measures

[[σ-Algebra|σ-algebras]] (denoted $\mathscr{F}$) are families of subsets that help us define [[Probability Measure|probability measures]], functions (denoted $\mathbb{P}(A)$) that let us measure the probability of a given event $A$.

Probability measures are also of special importance, hence why it is important to know [[Properties of a Probability Measure|their properties]].

## Combinations and Permutations

When selecting items from a set, we can have:

- A [[Combination|combination]], when we don't care about the order in which we select them.
- A [[Permutation|permutation]], when we do care about the order in which we select them.

### Principles of Counting

When selecting items from one set **or** another (both disjoint), the number of ways in which we can do so can be calculated by **adding** the cardinalities of both sets, according to the [[Addition Principle|addition principle]].

On the other hand, when selecting items from one set **and** another, the number of ways in which we can do so can be calculated by **multiplying** the cardinalities of both sets, according to the [[Multiplication Principle|multiplication principle]].

### Number of Combinations and Permutations

The number of permutations we can have depends on whether we have permutations [[Permutations with no Repetitions|with no repetitions]], [[Permutations with Repetitions|with repetitions]] or [[Permutations with Groups of Equal Elements|with groups of equal elements]].

The [[Number of Combinations|number of combinations]] is, in fact, the number of permutations with no repetitions divided by $k!$

## More Complex Events

When calculating the probability of an event $A$ **given** the occurrence of another event $B$, we say we have a [[Conditional Probability|conditional probability]].

We can express the probability of the intersection of various events as the product of several conditional probabilities. This is known as the [[Product Rule|product rule]].

When the occurrence of an event $A$ doesn't affect the occurrence of another event $B$, we say that $A$ and $B$ are [[Event Independence|independent]]. In that case, it also stands that $B$ doesn't affect $A$.

## Partitions, Total Probability and Bayes' Theorem

We can make [[Partition of a Sample Space|partitions in a sample space]]. From them, we can obtain:

- The [[Total Probability Formula|total probability formula]], which helps us obtain the probability of _any_ event in the sample set given a partition of the sample set.

- [[Bayes' Theorem|Bayes' theorem]], which helps us obtain the probability of an event given the probability of other related events.

# Unit 2: Random Variables

There are [[Theorems of Limits in a Probability Measure|various useful theorems that describe the behaviour of limits in a probability measure]].

## Random Variables

A [[Random Variable|random variable]] is a function that allows us to mathematically formalise the concept of randomness. They basically "translate" randomness into mathematical terms we can manipulate and study.

There are two types of random variables:

- [[Discrete Random Variable|Discrete random variables]], whose range is in a discrete set (whether finite or countably infinite).
- [[Absolutely Continuous Random Variable|Absolutely continuous random variables]], whose range is in an uncountably infinite set.

An [[Indicator Random Variable|indicating random variable]] is simply a random variable that tells us if a specific value is in an event.

## Density Functions

A [[Density Function|density function]] is a function that allows us to specify the probability of $X$ being a specific value (in the discrete case) or of $X$ falling within a particular range of values (in the continuous case, though indirectly).

## Distribution Functions

A [[Distribution Function|distribution function]] is a function that, in general, can be seen as the function that "accumulates" the values of a density function.

- Distribution functions have [[Properties of a Distribution Function|various properties]]. For instance, all distribution functions are [[Càdlàg Function|càdlàg]].
- Distribution functions can be defined at a value [[Distribution Function From the Left|from the left]].

Distribution functions [[Probabilities with a Distribution Function|help us find the probability]] that the given random variable falls within a specific interval of values.

## Moments

The [[Expected Value|expected value]] of a random variable corresponds, roughly, to the concept of the arithmetic mean of the outcomes of the random variable. Expected value has [[Properties of the Expected Value|several properties]].

When given a variable such that is defined according to another one (e.g. $Y = g(X)$), we can easily calculate its expected value with the [[Law of the Unconscious Statistician|law of the unconscious statistician]].

A [[Moment|moment]] of a random variable is a special value related to the behaviour of its probability distribution. Moments have an order $r$ ($r \geq 1$), and are either centred around the variable's expected value or around $0$.

The moment of order $2$ around the variable's expected value is better known as its [[Variance|variance]].

## Other Special Functions

The [[Moment-Generating Function|moment-generating function]] of a random variable is, as its name suggests, a function that lets us easily calculate its moments around $0$ when deriving and then evaluating it at $t = 0$.

Moment generating functions have [[Properties of a Moment-Generating Function|various properties]].

The [[Characteristic Function|characteristic function]] of a random variable is a function that's very similar to the moment-generating function, except that it involves complex numbers. Characteristic functions also have [[Properties of a Characteristic Function|various properties]].

# Unit 3: Notable Distributions

There are many notable probability distributions. Studying these distributions can help us solve problems more easily.

## Discrete Distributions

Let $X$ be a _discrete_ random variable.

1. $X$ has a [[Discrete Uniform Distribution|discrete uniform distribution]] when every one of $X$'s possible results are equally as probable.

2. $X$ has a [[Bernoulli Distribution|Bernoulli distribution]] when it handles the success or failure of a _single_ experiment.

3. $X$ has a [[Binomial Distribution|binomial distribution]] when it handles the success or failure of _multiple_ experiments of the same nature.

4. $X$ has a [[Geometric Distribution|geometric distribution]] when it handles the repetition of multiple success/failure experiments (of the same nature) until success is achieved. Beware: there is a normal geometric distribution and a very similar [[Shifted Geometric Distribution|shifted geometric distribution]].

5. $X$ has a [[Poisson Distribution|Poisson distribution]] when it handles the number of events that occur in a given time or space interval.

## Continuous Distributions

Let $X$ be a _continuous_ random variable.

1. $X$ has a [[Continuous Uniform Distribution|continuous uniform distribution]] when all intervals of a given length have the same probability.

2. A very common continuous distribution is the [[Normal Distribution|normal distribution]]. Many random variables that model natural, social or psychological phenomena have a normal distribution.

# Unit 4: Random Vectors

A [[Random Vector|random vector]] is the concept of a random variable generalised for multiple dimensions.

Random vectors have a [[Density Function of a Random Vector|(joint) density function]] and can also have [[Marginal Density Function|marginal]] and [[Conditional Density Function|conditional]] density functions.
