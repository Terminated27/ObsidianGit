---
aliases:
  - MAP estimator
---
#stats 
The Maximum a Posteriori (MAP) estimator is a method used to estimate the most likely values of unknown parameters in a statistical model. It is based on the principle of maximum likelihood, but incorporates prior knowledge about the parameters through a prior distribution. In this atomic note, we will discuss the concept of MAP estimation, its mathematical formulation, and provide step-by-step examples to illustrate its application.

## Definition

Let $\theta$ be a vector of unknown parameters and let $X$ be a [[set]] of observed data. The MAP estimator for $\theta$ is defined as:

$$\hat{\theta}_{MAP} = \arg\max_{\theta} p(\theta|X)$$

where $p(\theta|X)$ is the posterior distribution of $\theta$ given the observed data $X$. This can also be written as:

$$\hat{\theta}_{MAP} = \arg\max_{\theta} \frac{p(X|\theta)p(\theta)}{p(X)}$$

where $p(X|\theta)$ is the likelihood function and $p(\theta)$ is the prior distribution of $\theta$.

## The MAP Estimation Process

1. Specify the likelihood function $p(X|\theta)$ and the prior distribution $p(\theta)$.
2. Use Bayes' rule to calculate the posterior distribution $p(\theta|X)$.
3. Take the logarithm of both sides to simplify calculations.
4. Maximize the logarithm of the posterior distribution with respect to $\theta$.
5. The value of $\hat{\theta}_{MAP}$ that maximizes this expression is our MAP estimate.

## Example: Coin Tossing Experiment

Suppose we have conducted an experiment where we toss a coin 10 times and record whether it lands heads or tails each time. Let us assume that our coin has a probability $p$ of landing heads up. We want to use the data from this experiment to estimate the value of $p$. We can model this experiment using a binomial distribution, where the number of successes (heads) in 10 trials follows a binomial distribution with parameters $n=10$ and $p$.

The likelihood function for this experiment is given by:

$$p(X|\theta) = \binom{10}{x} p^x (1-p)^{10-x}$$

where $X$ is the number of heads observed in 10 trials.

Now, let us assume that we have some prior knowledge about the value of $p$. For example, we may know that the coin is biased towards landing heads up, so we expect $p$ to be greater than 0.5. We can model this prior knowledge using a beta distribution with parameters $\alpha=2$ and $\beta=1$, which has a mean of $\frac{\alpha}{\alpha+\beta} = \frac{2}{3}$.

The prior distribution for $p$ is given by:

$$p(\theta) = \frac{\Gamma(\alpha+\beta)}{\Gamma(\alpha)\Gamma(\beta)} p^{\alpha-1} (1-p)^{\beta-1}$$

where $\Gamma(\cdot)$ is the gamma function.

Using Bayes' rule, we can calculate the posterior distribution for $p$ as:

$$p(p|X) = \frac{p(X|p)p(p)}{p(X)}$$

Taking logarithms on both sides, we get:

$$\log p(p|X) = \log p(X|p) + \log p(p) - \log p(X)$$

Maximizing this expression with respect to $p$, we get:

$$\hat{p}_{MAP} = \frac{\alpha + x - 1}{\alpha + \beta + n - 2}$$

Substituting the values of $\alpha=2$, $\beta=1$, and $n=10$, we get:

$$\hat{p}_{MAP} = \frac{2 + x - 1}{2 + 1 + 10 - 2} = \frac{x+1}{13}$$

Therefore, our MAP estimate for $p$ is given by the number of heads observed plus one, divided by the total number of trials plus the sum of the prior parameters.

## Properties of MAP Estimators

- The MAP estimator is consistent, meaning that as the sample size increases, it converges to the true value of the parameter.
- It is also asymptotically efficient, meaning that it achieves the smallest possible [[variance]] among all consistent estimators.
- The choice of prior distribution can have a significant impact on the MAP estimate. A highly informative prior can lead to a biased estimate, while a non-informative prior may result in a less precise estimate.
- In some cases, the MAP estimator may not exist or may be difficult to calculate analytically. In such cases, numerical methods such as Markov Chain Monte Carlo (MCMC) can be used to obtain an approximate solution.

## Conclusion

The Maximum a Posteriori Estimator is a powerful tool for estimating unknown parameters in statistical models. By incorporating prior knowledge about the parameters through a prior distribution, it provides more accurate estimates compared to maximum likelihood estimation. However, careful consideration must be given to choosing an appropriate prior distribution to avoid biased estimates.