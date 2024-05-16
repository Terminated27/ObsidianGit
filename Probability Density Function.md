#stats 

In probability theory, a **Probability Density Function (PDF)** is a function that describes the likelihood of a [[continuous random variable]] falling within a particular range of values. The PDF, denoted as $f(x)$, must satisfy the following properties:

1. $f(x) \geq 0$ for all $x$
2. $\int_{-\infty}^{\infty} f(x)dx = 1$

The probability that a [[continuous random variable]] $X$ falls within an interval $[a,b]$ is given by:

$$P(a \leq X \leq b) = \int_{a}^{b} f(x)dx$$

## Key Theorems and Definitions

### Theorem: Mean of a [[Continuous Random Variable]]
The mean (or expected value) of a [[continuous random variable]] $X$ with PDF $f(x)$ is given by:

$$E[X] = \int_{-\infty}^{\infty} x f(x)dx$$

### Definition: Variance of a [[Continuous Random Variable]]
The variance of a [[continuous random variable]] $X$ with PDF $f(x)$ is given by:

$$Var(X) = E[(X - E[X])^2] = \int_{-\infty}^{\infty} (x - E[X])^2 f(x)dx$$

## Step-by-Step Example

Consider a [[continuous random variable]] $X$ with the following PDF:

$$f(x) = 
\begin{cases}
2x & 0 \leq x \leq 1 \\
0 & \text{otherwise}
\end{cases}
$$

### Step 1: Verify Properties
- We can verify that $f(x) \geq 0$ for all $x$.
- Calculate $\int_{0}^{1} 2xdx = [x^2]_{0}^{1} = 1$, satisfying the second property.

### Step 2: Calculate Mean
The mean of $X$ is given by:

$$E[X] = \int_{0}^{1} x(2x)dx = \int_{0}^{1} 2x^2dx = [\frac{2}{3}x^3]_{0}^{1} = \frac{2}{3}$$

### Step 3: Calculate Variance
The variance of $X$ is given by:
$$
\begin{align*}
Var(X) &= E[(X - E[X])^2] \\
&= \int_{0}^{1}(x - \frac{2}{3})^22xdx \\
&= \int_{0}{1}(4x^3 - \frac{8}{3}x^2 + \frac{4}{9})dx \\
&= [\frac{x^4}{4}-\frac{8}{9}\cdot\frac{x^3}{3}-\frac{4}{27}\cdot x]_0^1 \\
&= (\frac{1}{4}-\frac{8}{27}-\frac{4}{27}) \\
&= \frac{7}{54}
\end{align*}
$$
Thus, the mean and variance of the given PDF have been calculated.