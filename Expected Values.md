#stats 

In probability theory, the expected value of a [[random variable]] is a key concept that represents the [[average]] value of the variable over a large number of trials. It is denoted by $E[X]$ or $\mu_X$.

## Definition
The expected value of a [[discrete random variable]] $X$ with [[probability mass function]] $p(x)$ is given by:

$$E[X] = \sum_{x} x \cdot p(x)$$

For a [[continuous random variable]] $X$ with [[probability density function]] $f(x)$, the expected value is calculated as:

$$E[X] = \int_{-\infty}^{\infty} x \cdot f(x) dx$$

## Properties
1. Linearity of Expectation: For constants $a$ and $b$, and random variables $X$ and $Y$, we have:

$$
\begin{align}
E[aX + bY] &= aE[X] + bE[Y]\\
\\
E[aXbY] &= aE[X] \times bE[Y]
\end{align}
$$

2. Expectation of a Constant: For any constant $c$, $E[c] = c$.

3. Expectation of a Function: If $g(X)$ is a function of [[random variable]] $X$, then:

$$E[g(X)] = \sum_{x} g(x) \cdot p(x) \quad \text{(discrete)}$$

or 

$$E[g(X)] = \int_{-\infty}^{\infty} g(x) \cdot f(x) dx \quad \text{(continuous)}$$

## Example
Consider rolling a fair six-sided die. Let the [[random variable]] $X$ represent the outcome of the roll. The expected value of $X$ can be calculated as:

$$E[X] = 1\left(\frac{1}{6}\right) + 2\left(\frac{1}{6}\right) + 3\left(\frac{1}{6}\right) + 4\left(\frac{1}{6}\right) + 5\left(\frac{1}{6}\right) + 6\left(\frac{1}{6}\right) = 3.5$$

Therefore, on [[average]], we expect the outcome of rolling a fair six-sided die to be 3.5.