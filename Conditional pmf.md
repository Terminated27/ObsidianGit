

The [[conditional probability]] mass function ([[Probability Mass Function|pmf]]) is a concept in probability theory that describes the probability distribution of a [[random variable]] given certain conditions. It is denoted as $P(X = x | Y = y)$, which represents the probability that the [[random variable]] $X$ takes on a specific value $x$ given that another [[random variable]] $Y$ takes on a specific value $y$.

## Definition
The conditional [[Probability Mass Function|pmf]] of a discrete [[random variable]] $X$ given another discrete [[random variable]] $Y$ is defined as:

$$P(X = x | Y = y) = \frac{P(X = x, Y = y)}{P(Y = y)}$$

where:
- $P(X = x, Y = y)$ is the joint [[probability mass function]] of $X$ and $Y$
- $P(Y = y)$ is the [[marginal probability]] mass function of $Y$

## Key Theorem: Law of Total Probability
The law of total probability states that for any partition $\{B_1, B_2, \ldots, B_n\}$ of the [[sample space]]:

$$P(A) = \sum_{i=1}^{n} P(A | B_i) \cdot P(B_i)$$

for any [[event]] A.

## Example
Suppose we have two dice, one fair and one loaded. Let X be the outcome of the fair die and Y be the outcome of the loaded die. The joint [[Probability Mass Function|pmf]] is given by:

$$P(X=x,Y=y)=\begin{cases}
\frac{1}{36}, & \text{if } x,y \in \{1,2,3,4,5,6\}\\
0, & \text{otherwise}
\end{cases}$$

If we want to find the conditional [[Probability Mass Function|pmf]] of X given Y=3:

$$P(X=x|Y=3)=\begin{cases}
\frac{1}{6}, & \text{if } x \in \{1,2,3,4,5,6\}\\
0, & \text{otherwise}
\end{cases}$$

This means that given Y=3 on the loaded die, X has an equal chance of being any number from 1 to 6 on the fair die.

By understanding conditional pmfs and using them in conjunction with joint and marginal probabilities, we can gain deeper insights into the relationships between random variables in probabilistic scenarios.