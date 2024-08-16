---
type: 🏫
tags:
  - MAC/5/E1
---

# Unit 1: Introduction to Statistics

[[Statistics]] is the science of collecting, organising, summarising and analysing data to draw conclusions from it. It can be divided in two branches:

- [[Descriptive Statistics|Descriptive statistics]], which describes, resumes and organises data.
- [[Inferential Statistics|Inferential statistics]]. which draw conclusions from said data.

As with many disciplines, the [[Scientific Method in Statistics|scientific method can be easily applied to statistics]].

## Basic Concepts

A [[Population|population]] is a set of elements in which we're interested. A [[Sample|sample]] is a subset of a population.

A [[Variable (Statistics)|variable]] is a feature of a population. Variables can measure both [[Quantitative Variable|quantities]] and [[Qualitative Variable|qualities]]. The set of observations for a specific variable in a given population is called [[Data (Statistics)|data]].

## Measures

### Measures of Central Tendency

A [[Measure of Central Tendency|measure of central tendency]] is a value in a set of data that can be described as being in the centre of the (sorted) data. The most common measures of central tendency are the [[Arithmetic Mean|arithmetic mean]], the [[Weighted Mean|weighted mean]], the [[Median|median]] and the [[Mode|mode]].

In the case of the arithmetic mean, it is also possible to calculate it when we have [[Arithmetic Mean for a Set of Frequencies|a table of frequencies]] or [[Arithmetic Mean for Grouped Data|groups of data with class marks]]. Similarly, we can calculate the [[Median for a Set of Frequencies|median for a table of frequencies]].

### Measures of Position

A [[Quantile|quantile]] is a value that serves as a measure of position. They can be seen as the value up to which a random variable accumulates a given density. Percentiles, quartiles and deciles are specific cases of quantiles.

### Measures of Dispersion

A [[Measure of Dispersion|measure of dispersion]] is a value that helps us describe how disperse the mass of a variable is. [[Variance#As a Measure of Dispersion|Variance]], [[Enirkesto/E1/Standard Deviation|standard deviation]], [[Mean Deviation|mean deviation]] and [[Range (Measure of Dispersion)|range]] are all examples of measures of dispersion.

### Measures of Shape

A [[Enirkesto/E1/Measure of Shape|measure of shape]] is a value that helps us describe the shape that a variable's mass has. [[Moment|Moments]], [[Skewness|skewness]], [[Kurtosis|kurtosis]] and [[Excess Kurtosis|excess kurtosis]] are examples of measures of shape.

### Measures of Association

A [[Measure of Association|measure of association]] is a value that quantifies the relationship between two or more variables. [[Covariance]] and [[Pearson's Correlation Coefficient|Pearson's correlation coefficient]] are examples of measures of association.

## Graphical Representations

[[Graphical Representations of Statistical Data|Statistical data can be represented graphically]] in many types of graphs, which include, but are not limited to:

- [[Bar Chart|Bar charts]], where classes of a variable are associated with a frequency bar.
- [[Histogram|Histograms]], where values are ordered.
- [[Dispersion Graph|Dispersion graphs]], which show the relation between _two_ variables.
- [[Bubble Graph|Bubble graphs]], which show the relation between _three_ variales.
- [[Time Series|Time series]], which show the evolution of a variable across time.
- [[Box Plot|Box plots]], which summarise a series of numerical data with the help of quartiles.

# Unit 2: Methods for Obtaining Functions of Random Variables

## Probability Theory

> [!info] (Not so Brief) Probability Theory Review
> A brief review on probability theory was seen, which included the concepts of [[Random Variable|random variable]] ([[Discrete Random Variable|discrete]] and [[Absolutely Continuous Random Variable|continuous]]), [[Density Function|density function]], [[Distribution Function|distribution function]], [[Random Vector|random vector]], and [[Moment-Generating Function|moment-generating function]], to name just a few.
>
> I created no new notes for these concepts, since I had already seen all of them during my **[[Probabilidad]]** course (🏫). I did improve and edit some of them, however.

When defining a random variable in terms of another, we can [[Density and Distribution Function of a Dependent Random Variable|find its density and distribution function by using one of two methods]].

## Collections of iid Random Variables

We say that a collection of random variables is [[Independent and Identically Distributed Random Variables|iid]] when all of them are mutually independent and have the same probability distribution.

More specifically, when sampling a population and describing the random variables whose [[Random Variable Realisation|realisations]] we have obtained as samples, we refer to a collection of iid random variables as a [[Random Sample|random sample]].

When ordering the random variables in a random sample according to their realisations, we can define the concept of [[Order Statistic|order statistics]].

## More Probability Distributions

When having a collection of random variables that follow a standard normal distribution, the random variable that results from adding their squares up follows what we call a [[Chi-Squared Distribution|chi-squared distribution]] (denoted, of course, with the Greek letter chi $\chi$).

[[Student's T-Distribution|Student's t-distribution]] describes the distribution of a random variable that results from operating a normally distributed random variable with a chi-squared distributed one.

Similarly, when operating two random variables that follow a chi-squared distribution, the resulting random variable has an [[F Distribution|F distribution]].

# Unit 3: Sampling Distributions

## Random Samples, Sample Statistics and Parameters

When sampling a population and describing the random variables whose [[Random Variable Realisation|realisations]] we have obtained as samples, we refer to a collection of iid random variables as a [[Random Sample|random sample]].

A [[Sample Statistic|sample statistic]] ("_estadístico_" in Spanish) is a random variable that results from passing a random sample through a function. The corresponding distributions of such random variables are called [[Sampling Distribution|sampling distributions]].

A [[Parameter (Statistics)|parameter]] is a numerical characterisation of a population that describes partially or completely its probability distribution. The set of all possible values that a parameter can have is called its [[Parameter Space|parameter space]].

## Expected Value, Variance and Moment-Generating Function Theorems

When defining a random variable as the sum of the random variables in a random sample multiplied by some scalar each, [[Moment-Generating Function of the Sum of the Random Variables in a Random Sample|its moment-generating function can be easily determined]].

When we know the expected value and variance of the random variables of our random sample, then obtaining the [[Expected Value and Variance of the Mean of a Random Sample|expected value and variance of the mean of our random sample]] is easy.

## Central Limit Theorem

The [[Central Limit Theorem|central limit theorem]] is an important theorem that allows us to use a standard normal distribution to approximate a sum of $n$ iid random variables with _any_ distribution.

## Sample Variance Theorems

Given a normally distributed random sample, [[Sampling Distribution of the Variance of a Normally Distributed Random Sample|we can use a chi-squared distribution to work with its variance]]. We can do something similar [[Sampling Distribution of the Variance of a Normally Distributed Random Sample with an Unknown Expected Value|even when we don't know the expected value of the random variables]], albeit with a slightly different sample variance.

# Unit 4: Point and Interval Estimation

## Estimators

Given a random sample characterised by a parameter, an [[Estimator|estimator]] is a sample statistic that aims to estimate (i.e. give an approximation of) such a parameter.

An estimator can be:

- [[Unbiased Estimator|Unbiased]] when its expected value is equal to the parameter it estimates.
- [[Asymptotically Unbiased Estimator|Asymptotically unbiased]] (in the case of a sequence of estimators) when, as the size of the sequence increases, the expected values converge to the estimated parameter.
- [[Efficient Estimator|More efficient than others]] when their variance is smaller.
- [[Consistent Estimator|Consistent]] (in the case of a sequence of estimators) when, as the size of the sequence increases, they converge to the estimated parameter.

The [[Bias (Statistics)|bias]] of an estimator is the difference between its expected value and the parameter it estimates. The [[Mean Squared Error|mean squared error (MSE)]] is the expected value of the square of this difference.

## Obtaining Estimators

We can use several methods to obtain estimators for a given parameter:

- The [[Moments Method for Obtaining Estimators|moments method]] consists of equating the population moments with their corresponding sample moments, and then solving the resulting equation(s).
- The [[Maximum Likelihood Method for Obtaining Estimators|maximum likelihood method]] consists of maximising the random sample's likelihood function.
	- As its name suggests, this method uses a random sample's [[Likelihood Function|likelihood function]], which is the product of the density functions of each random variable in the sample.

## Cramér-Rao Lower Bound

Given an estimator $T$, the [[Cramér-Rao Lower Bound|Cramér-Rao lower bound]] provides a lower bound for $\mathrm{Var}(T)$.

An estimator $T$ is said to be a [[Uniformly Minimum-Variance Unbiased Estimator|uniformly minimum-variance unbiased (UMVUE) estimator]] when (1) it's unbiased and (2) its Cramér-Rae lower bound is _equal_ to $\mathrm{Var}(T)$.
