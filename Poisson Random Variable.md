#stats 
A Poisson [[random variable]] is a [[discrete random variable]] that represents the number of events occurring in a fixed interval of time or space, given that these events occur with a constant average rate and are independent of the time since the last [[event]]. 

## [[Probability Mass Function]] ([[Probability Mass Function|PMF]])

The [[probability mass function]] of a Poisson [[random variable]] $X$ with parameter $\lambda > 0$ is given by:

$$
P(X = k) = \frac{e^{-\lambda} \lambda^k}{k!}, \quad k = 0, 1, 2, \ldots
$$

where $e$ is Euler's number approximately equal to $2.71828$.

## Mean and Variance

The mean and variance of a Poisson [[random variable]] $X$ are both equal to the parameter $\lambda$, denoted as $\text{E}[X] = \lambda$ and $\text{Var}[X] = \lambda$.
This can be used backwards to find the value of $\lambda$
## Key Theorem: Poisson Approximation to Binomial Distribution

When the number of trials $n$ in a binomial distribution is large and the probability of success $p$ is small such that $\lambda = np$ remains constant, then the binomial distribution can be approximated by a Poisson distribution with parameter $\lambda$. This approximation becomes more accurate as $n$ becomes larger.

## Example

Suppose the number of customers arriving at a store follows a Poisson distribution with an average rate of 5 customers per hour. What is the probability that exactly 3 customers arrive in the next hour?

Using the [[Probability Mass Function|PMF]] formula:

$$
P(X = 3) = \frac{e^{-5} \cdot 5^3}{3!} \approx 0.14037
$$

Therefore, the probability of exactly 3 customers arriving in the next hour is approximately 0.14037.

$$
P(X > 20) = \sum_{k=21}^\infty \frac{e^{-10} \cdot 10^k}{k!}
$$
