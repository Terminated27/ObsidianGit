#stats 

In probability theory, multiple random variables refer to a collection of two or more random variables defined on the same probability space. Understanding the joint behavior of multiple random variables is crucial in various statistical and [[machine learning]] applications.

## Joint Probability Distribution

The joint probability distribution of two random variables $X$ and $Y$ is denoted as $P(X=x, Y=y)$ or simply $P(x, y)$. It describes the probability that $X=x$ and $Y=y$ simultaneously. For [[Discrete Random Variable]], the joint [[probability mass function]] is defined as:

$$
P(X=x, Y=y) = P(X=x \cap Y=y)
$$

For [[Continuous Random Variable]], the joint [[probability density function]] is defined similarly.

## [[Marginal Probability]] Distribution

The [[marginal probability]] distribution of a single [[random variable]] from a [[set]] of multiple random variables can be obtained by summing (or integrating) over all possible values of the other variables. For example, the marginal distribution of $X$ is given by:

$$
P(X=x) = \sum_{y} P(X=x, Y=y) \quad \text{(discrete case)}
$$

$$
f_X(x) = \int_{-\infty}^{\infty} f_{XY}(x,y) dy \quad \text{(continuous case)}
$$

## [[Conditional Probability]] Distribution

The [[conditional probability]] distribution of one [[random variable]] given another is defined as:

$$
P(Y=y|X=x) = \frac{P(X=x,Y=y)}{P(X=x)}
$$

This allows us to model the relationship between multiple random variables.

## Independence of Random Variables

Two random variables $X$ and $Y$ are independent if their joint probability distribution can be expressed as the product of their marginal distributions:

$$
P(X,Y) = P(X)P(Y)
$$

This implies that knowing the value of one variable provides no information about the other.

## [[Covariance]] and [[Correlation]]

[[Covariance]] measures how two random variables vary together from their means, while [[correlation]] measures how they vary relative to their standard deviations. They are defined as:

$$
\text{Cov}(X,Y) = E[XY]-E[X]\times E[Y]
$$

$$
\rho_{XY} = \frac{\text{Cov}(X,Y)}{\sigma_X\sigma_Y}
$$

Understanding these measures helps in analyzing the relationship between multiple random variables.

Overall, studying multiple random variables provides valuable insights into complex systems and enables us to make informed decisions based on probabilistic models.