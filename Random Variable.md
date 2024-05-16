#stats
A random variable is a variable whose possible values are outcomes of a random phenomenon. It can be discrete or continuous, depending on whether its possible values are [[Countable]] or uncountable.

## [[Discrete Random Variable]]

A [[discrete random variable]] has a [[Countable]] number of possible values. The [[probability mass function]] ([[Probability Mass Function|PMF]]) of a [[discrete random variable]] $X$ is defined as:

$$
P(X = x) = p(x)
$$

where $p(x)$ represents the probability that the random variable takes on the value $x$. The [[Probability Mass Function|PMF]] must satisfy two properties:

1. $\sum_{x} p(x) = 1$ for all possible values of $X$
2. $0 \leq p(x) \leq 1$ for all possible values of $X$

## [[Continuous Random Variable]]

A [[continuous random variable]] takes on an uncountable number of possible values. Instead of a [[Probability Mass Function|PMF]], it has a [[probability density function]] (PDF). The PDF of a [[continuous random variable]] $X$ is denoted by $f(x)$ and satisfies:

$$
\int_{-\infty}^{\infty} f(x) dx = 1
$$

The probability that a [[continuous random variable]] falls within a certain interval $[a,b]$ is given by the [[integral]] of the PDF over that interval:

$$
P(a \leq X \leq b) = \int_{a}^{b} f(x) dx
$$

## Expected Value

The expected value or mean of a random variable $X$, denoted by $\mu$, is defined as:

$$
E[X] = \mu = \sum_{x} x \cdot p(x) \quad (\text{for discrete } X)
$$

or 

$$
E[X] = \mu = \int_{-\infty}^{\infty} x \cdot f(x) dx  \quad (\text{for continuous } X)
$$

## [[Variance]] and Standard Deviation

The variance of a random variable measures how spread out its values are around the mean. It is defined as:

$$
Var(X) = E[(X - E[X])^2]
$$
or
$$
Var(X) = E[X^2] - E[X]^2
$$
and the standard deviation is the square root of the variance.

## Example: 

Let's consider a fair six-sided die as our random variable. The [[Probability Mass Function|PMF]] for this [[discrete random variable]] would be:

- $p(1)=\frac{1}{6}, p(2)=\frac{1}{6}, p(3)=\frac{1}{6}, p(4)=\frac{1}{6}, p(5)=\frac{1}{6}, p(6)=\frac{1}{6}$

The expected value would be calculated as:

$$
E[X] = 1*\frac{1}{6} + 2*\frac{1}{6} + 3*\frac{1}{6} + 4*\frac{1}{6} + 5*\frac{1}{6} + 6*\frac{1}{6}
     = \frac{21}{6}
     = 3.5
$$