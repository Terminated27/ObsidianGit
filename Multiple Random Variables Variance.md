

In probability theory, the [[variance]] of a [[random variable]] is a measure of how much its values vary from the mean. When dealing with [[multiple random variables]], we can extend this concept to calculate the [[variance]] of their joint distribution. In this atomic note, we will explore the concept of [[multiple random variables]] [[variance]] and its properties.

## Definition

Let $X_1, X_2, ..., X_n$ be $n$ random variables with joint probability distribution $f(x_1,x_2,...,x_n)$. The [[variance]] of these random variables is defined as:

$$Var(X_1,X_2,...,X_n) = E\bigg[\bigg(\sum_{i=1}^n(X_i-\mu_i)^2\bigg)\bigg]$$

where $\mu_i = E[X_i]$ is the mean of $X_i$. This can also be written as:

$$Var(X_1,X_2,...,X_n) = \sum_{i=1}^n \sum_{j=1}^n Cov(X_i,X_j)$$

where $Cov(X_i,X_j)$ is the covariance between $X_i$ and $X_j$.

## Properties

The following properties hold for [[multiple random variables]] [[variance]]:

- **Linearity:** If $a$ and $b$ are constants and $Y = aX + b$, then $Var(Y) = a^2 Var(X)$.
- **Sum of Independent Random Variables:** If $X$ and $Y$ are independent random variables, then $Var(X+Y) = Var(X) + Var(Y)$.
- **[[Covariance]] and Independence:** If two random variables are independent, their [[covariance]] is 0. Hence, if all pairs of random variables in a [[set]] are independent, then their variances add up.
- **Symmetry:** $Var(X_1,X_2,...,X_n) = Var(X_{\pi(1)},X_{\pi(2)},...,X_{\pi(n)})$ for any permutation $\pi$ of the indices $1,2,...,n$.

## Example

Let's consider two non-independent random variables $X$ and $Y$, with means $\mu_X = 3$ and $\mu_Y = 5$, and variances $Var(X) = 4$ and $Var(Y) = 9$. We can calculate the [[variance]] of their sum as follows:



$$
Var(X + Y) = Var(X) + Var(Y) + 2Cov(X,Y)
$$

## Theorem: [[Variance]] of a Linear Combination

If $X_1, X_2, ..., X_n$ are random variables with joint probability distribution $f(x_1,x_2,...,x_n)$ and constants $a_1,a_2,...,a_n$, then the [[variance]] of the linear combination $Y = a_1X_1 + a_2X_2 + ... + a_nX_n$ is given by:

$$Var(Y) = \sum_{i=1}^n \sum_{j=1}^n a_i a_j Cov(X_i,X_j)$$

## Proof

We can write the linear combination as:

$$Y = \sum_{i=1}^n a_i X_i$$

Using the properties of [[variance]], we have:

$$Var(Y) = Var\bigg(\sum_{i=1}^n a_i X_i\bigg)$$
$$= \sum_{i=1}^n Var(a_i X_i) + \sum_{i \neq j} Cov(a_i X_i,a_j X_j)$$
$$= \sum_{i=1}^n a_i^2 Var(X_i) + \sum_{i \neq j} a_i a_j Cov(X_i,X_j)$$
$$= \sum_{i=1}^n \sum_{j=1}^n a_i a_j Cov(X_i,X_j)$$

Hence, the theorem is proved.

## Conclusion

In this atomic note, we have explored the concept of [[multiple random variables]] [[variance]] and its properties. We have seen that the [[variance]] of [[multiple random variables]] is simply the sum of their individual variances and covariances. The theorem for calculating the [[variance]] of a linear combination of random variables is also useful in many applications. 