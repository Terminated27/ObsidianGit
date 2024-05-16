#stats 
![[Pasted image 20240304091758.png]]
In probability theory, a **discrete [[random variable]]** is a [[random variable]] that can take on a [[Countable]] number of distinct values. It is characterized by its [[probability mass function]] ([[Probability Mass Function|PMF]]), which assigns probabilities to each possible value the [[random variable]] can take.

## Key Theorems and Definitions

### [[Probability Mass Function]] ([[Probability Mass Function|PMF]])

The [[Probability Mass Function|PMF]] of a discrete [[random variable]] $X$ is defined as:

$$
P(X = x) = P(X \in \{x\})
$$

where $x$ is a specific value that $X$ can take.

### Expected Value

The expected value or mean of a discrete [[random variable]] $X$ is given by:

$$
E[X] = \sum_{x} x \cdot P(X = x)
$$

### Variance

The variance of a discrete [[random variable]] $X$ is given by:

$$
Var(X) = E[(X - E[X])^2] = \sum_{x} (x - E[X])^2 \cdot P(X = x)
$$
$$
Var(X) = E[X^2]-E[X]^2
$$

## Step-by-Step Example

Consider a fair six-sided die. Let $X$ be the [[random variable]] representing the outcome of rolling the die.

1. **[[Probability Mass Function]]:**

The [[Probability Mass Function|PMF]] of $X$ is given by:

$$
P(X = x) =
\begin{cases}
\frac{1}{6}, & \text{if } x \in \{1, 2, 3, 4, 5, 6\} \\
0, & \text{otherwise}
\end{cases}
$$

2. **Expected Value:**

The expected value of $X$ is calculated as:

$$
E[X] = \sum_{x=1}^{6} x \cdot P(X = x) = 3.5
$$

3. **Variance:**

The variance of $X$ is calculated as:

$$
Var(X) = E[(X - E[X])^2] = \sum_{x=1}^{6} (x - 3.5)^2 \cdot P(X = x) = 2.92
$$

By understanding and applying these key concepts related to discrete random variables, one can analyze and make predictions about various probabilistic scenarios involving [[Countable]] outcomes.