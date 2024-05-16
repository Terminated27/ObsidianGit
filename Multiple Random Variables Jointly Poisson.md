

In the context of probability theory, when dealing with [[multiple random variables]] that follow a Poisson distribution, we refer to them as **[[Multiple Random Variables]] Jointly Poisson**. This concept is particularly useful in scenarios where events occur independently and at a constant rate.

## Definition
Let $X_1, X_2, ..., X_n$ be $n$ random variables. We say that these random variables are jointly Poisson distributed if the following conditions hold:
1. Each individual [[random variable]] $X_i$ follows a Poisson distribution with parameter $\lambda_i$, i.e., $X_i \sim \text{Poisson}(\lambda_i)$.
2. The random variables are independent of each other.

## Theorem: Joint [[Probability Mass Function]]
The joint [[probability mass function]] ([[Probability Mass Function|pmf]]) of [[multiple random variables]] jointly Poisson is given by:
$$P(X_1 = x_1, X_2 = x_2, ..., X_n = x_n) = \prod_{i=1}^{n} \frac{e^{-\lambda_i} \lambda_i^{x_i}}{x_i!}$$

## Example
Suppose we have two random variables $X$ and $Y$, where $X \sim \text{Poisson}(2)$ and $Y \sim \text{Poisson}(3)$. If these two random variables are jointly Poisson distributed, then the joint [[Probability Mass Function|pmf]] is:
$$P(X = x, Y = y) = e^{-2} \frac{2^x}{x!} e^{-3} \frac{3^y}{y!}$$

This allows us to calculate the probability of specific combinations of values for both random variables.

In conclusion, understanding [[Multiple Random Variables]] Jointly Poisson provides a powerful tool for modeling and analyzing scenarios where multiple independent events occur at constant rates.