#stats 

In probability theory, multiple [[Discrete Random Variable]] refer to a collection of random variables that can take on discrete values. Let $X_1, X_2, \ldots, X_n$ be $n$ [[Discrete Random Variable]] defined on a common probability space $(\Omega, \mathcal{F}, P)$.

## Joint [[Probability Mass Function]] ([[Probability Mass Function|PMF]])

The joint [[probability mass function]] ([[Probability Mass Function|PMF]]) of multiple [[Discrete Random Variable]] is defined as:

$$
P(X_1 = x_1, X_2 = x_2, \ldots, X_n = x_n) = P(X_1 = x_1) \cdot P(X_2 = x_2) \cdots P(X_n = x_n)
$$

for all possible values $x_1, x_2, \ldots, x_n$.

To find each value in [[Probability Mass Function|PMF]] table:

$$
P_{x_k,y_j}
$$

## [[Marginal Probability]]

The [[marginal probability]] of a single [[random variable]] in the context of multiple [[Discrete Random Variable]] can be obtained by summing or marginalizing over all other variables. For example, the marginal [[Probability Mass Function|PMF]] of $X_1$ is given by:

$$
P(X_1 = x_1) = \sum_{x_2} \sum_{x_n} P(X_1 = x_1, X_2 = x_2, \ldots, X_n = x_n)
$$

## [[Conditional Probability]]

The [[conditional probability]] of one [[random variable]] given another in the context of multiple [[Discrete Random Variable]] is defined as:

$$
P(X_i = x_i | X_j = x_j) = \frac{P(X_i=x_i,X_j=x_j)}{P(X_j=x_j)}
$$

for $i\neq j$.
## Independence

Multiple [[Discrete Random Variable]] $X_1, X_2, \ldots, X_n$ are said to be independent if and only if their joint [[Probability Mass Function|PMF]] factorizes into the product of their individual PMFs:

$$
P(X_1=x_1,X_2=x_{2},\ldots,X_{n}=x_{n})=P(X_{1}=x_{1})\cdot P(X_{2}=x_{2})\cdots P(X_{n}=x_{n})
$$

for all possible values $x_{i}$.

[[Multiple random variables]] are considered independent if the probability of all of them occurring together is equal to the product of the probabilities of each one occurring individually.
## Example 1: 

Suppose we have two [[Discrete Random Variable]] $X$ and $Y$ with the following joint [[Probability Mass Function|PMF]]:

|     | Y=0  | Y=1  | Y=2  |
| --- | ---- | ---- | ---- |
| X=0 | 0.3  | 0.15 | 0.05 |
| X=1 | 0.15 | 0.25 | 0.10 |

Determine the marginal PMFs for $X$ and $Y$, and check if they are independent.

### Solution:

The marginal PMFs for $X$ and $Y$ can be calculated by summing over all possible values:

For $X$: 

$$
P(X=0) = 0.3 + 0.15 + 0.05 = 0.5 \\
P(X=1) = 0.15 + 0.25 + 0.10 = 0.5
$$

For $Y$: 

$$
P(Y=0) = 0.3 + 0.15 = 0.45 \\
P(Y=1) = 0.15 + 0.25 = 40 \\
P(Y=2) - 05 + .10 - .15
$$

To check for independence:
Since the joint [[Probability Mass Function|PMF]] factorizes into the product of marginal PMFs ($P(x,y)=p(x)p(y)$), we can conclude that the random variables are independent.

This example illustrates how to compute marginal probabilities and test for independence in the context of multiple [[Discrete Random Variable]] using their joint [[Probability Mass Function|PMF]].




## Example 2

Let's say we have two random variables X and Y with the following joint [[probability mass function]] ([[Probability Mass Function|pmf]]) chart

|   | Y=1 | Y=2 | Y=3 |
|---|-----|-----|-----|
| X=1 | 0.1 | 0.2 | 0.1 |
| X=2 | 0.2 | 0.1 | 0.1 |

Now, let's calculate the [[conditional probability]] of X=1 given Y=2 using the formula provided:

$$
P(X=1 | Y=2) = \frac{P(X=1, Y=2)}{P(Y=2)}
$$

From the joint [[Probability Mass Function|pmf]] chart, we can see that P(X=1, Y=2) = 0.2 and P(Y=2) = 0.2 + 0.1 = 0.3.

Therefore,

$$
P(X=1 | Y=2) = \frac{0.2}{0.3} = \frac{2}{3}
$$

So, the [[conditional probability]] of X being equal to 1 given that Y is equal to 2 is $\frac{2}{3}$.
