---
aliases:
  - PMF
---

#stats

In probability theory and statistics, a Probability Mass Function (PMF) is a function that gives the probability that a [[discrete random variable]] is equal to a specific value. The PMF of a [[random variable]] $X$ is denoted as $P(X = x)$, where $x$ is the specific value.

The PMF must satisfy the following properties:
1. $0 \leq P(X = x) \leq 1$ for all values of $x$.
2. $\sum_{x} P(X = x) = 1$, where the sum is taken over all possible values of $X$.

## Key Theorems
### Law of Total Probability
For any partition of the [[sample space]] into events $B_1, B_2, ..., B_n$, the total probability of an [[event]] $A$ can be expressed as:
$$P(A) = \sum_{i=1}^{n} P(A \cap B_i)$$

### Bayes' Theorem
Bayes' Theorem relates the conditional and marginal probabilities of two events. For events $A$ and $B$, it can be stated as:
$$P(A|B) = \frac{P(B|A)P(A)}{P(B)}$$

## Step-by-Step Example
Consider a fair six-sided die. Let $X$ be a [[random variable]] representing the outcome of rolling the die. The PMF of $X$ can be defined as:
$$P(X = x) = \frac{1}{6}, \text{ for } x = 1,2,3,4,5,6$$

To find the probability that the outcome is even ($X$ is even), we can calculate:
$$P(X \text{ is even}) = P(X=2) + P(X=4) + P(X=6) = \frac{1}{6} + \frac{1}{6} + \frac{1}{6} = \frac{1}{2}$$

This example illustrates how to use the PMF to calculate probabilities for [[Discrete Random Variable]].

By understanding Probability Mass Functions and their properties, we can analyze and predict outcomes in various probabilistic scenarios with [[Discrete Random Variable]].