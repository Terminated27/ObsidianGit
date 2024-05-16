#stats 

Continuous random variables are variables that can take on any value within a specified range. They are characterized by a [[probability density function]] (pdf) rather than a [[probability mass function]]. The probability of a continuous [[random variable]] falling within a specific interval is given by the [[integral]] of its pdf over that interval.

## [[Probability Density Function]] (pdf)
([[Derivative]] of [[Cumulative Distribution Function]])
The pdf of a continuous [[random variable]] $X$ is denoted as $f(x)$ and satisfies the following properties:

1. $f(x) \geq 0$ for all $x$
2. $\int_{-\infty}^{\infty} f(x)dx = 1$

The probability that $X$ falls in the interval $(a,b)$ is given by:

$$P(a \leq X \leq b) = \int_{a}^{b} f(x)dx$$

## Expected Value and Variance

The expected value of a continuous [[random variable]] $X$ is given by:

$$E[X] = \int_{-\infty}^{\infty} x f(x)dx$$

And the variance is calculated as:

$$Var(X) = E[X^2] - (E[X])^2 = \int_{-\infty}^{\infty} x^2 f(x)dx - (E[X])^2$$

## Key Theorems

### Law of the Unconscious Statistician (LOTUS)

The expected value of a function $g(X)$ of a continuous [[random variable]] $X$ is given by:

$$E[g(X)] = \int_{-\infty}^{\infty} g(x)f(x)dx$$

### [[Central Limit Theorem]]

For a sequence of independent and identically distributed random variables, their sum tends towards a normal distribution as the sample size increases, regardless of the distribution of individual variables.

## Step-by-Step Example

**Example:** Let $X$ be a continuous [[random variable]] with pdf:

$$f(x) = 
\begin{cases}
\frac{1}{3}(x+1)^2 & -1 \leq x \leq 0 \\
\frac{1}{3}(1-x)^2 & 0 < x \leq 1 \\
0 & otherwise
\end{cases}
$$

Find $E[X]$.

**Solution:**

We have:
$$
\begin{align*}
E[X] &= \int_{-\infty}^{\infty} x f(x)dx \\
&= \int_{-1}^{0} x \cdot \frac{1}{3}(x+1)^2 dx + \int_{0}^{1} x \cdot \frac{1}{3}(1-x)^2 dx \\
&= ... \\ % Perform [[integration]]
&= -\frac{5}{18}
\end{align*}
$$

Therefore, the expected value of $X$ is $-\frac{5}{18}$.

Continuous random variables play a crucial role in various fields such as statistics, physics, and finance. Understanding their properties and calculations can help in making informed decisions based on probabilistic outcomes.