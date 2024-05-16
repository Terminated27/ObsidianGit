---
aliases:
  - MMSE
---
#stats 
# Minimum Mean Square Estimator

The Minimum Mean Square Estimator (MMSE) is a method used in statistical signal processing to estimate an unknown quantity based on observed data. It is a popular technique due to its simplicity and effectiveness in minimizing estimation errors.

## Definition

The MMSE estimator is defined as the estimator that minimizes the [[mean square error]] (MSE) between the estimated value and the true value of the unknown quantity. In other words, it is the estimator that provides the best possible trade-off between bias and [[variance]].

## Theorem 1: MMSE Estimator

Let X be a [[random variable]] representing the observed data, Y be a [[random variable]] representing the unknown quantity to be estimated, and Z be a [[random variable]] representing the estimated value. Then, the MMSE estimator of Y given X is given by:

$$Z_{MMSE} = E[Y|X]$$

In other words, the MMSE estimator is equal to the conditional expectation of Y given X.

## Theorem 2: Orthogonality Principle

The Orthogonality Principle states that for any random variables X and Y, their [[covariance]] is equal to zero if and only if they are uncorrelated. Mathematically,

$$Cov(X,Y) = 0 \iff E[XY] = E[X]E[Y]$$

This principle plays a crucial role in deriving the MMSE estimator.

## Step-by-Step Example

Let us consider an example where we have two random variables X and Y with known means and variances. We want to estimate Y using X as our observation.

Step 1: Calculate [[Covariance]]
First, we calculate the [[covariance]] between X and Y using their known means and variances:

$$Cov(X,Y) = E[XY] - E[X]E[Y] = \rho\sigma_X\sigma_Y - \mu_X\mu_Y$$

where $\rho$ is the [[correlation]] coefficient between X and Y, and $\sigma_X$ and $\sigma_Y$ are the standard deviations of X and Y, respectively.

Step 2: Calculate MMSE Estimator
Using Theorem 1, we can calculate the MMSE estimator as:

$$Z_{MMSE} = E[Y|X] = \mu_Y + \frac{Cov(X,Y)}{\sigma_X^2}(X - \mu_X)$$

Substituting the previously calculated [[covariance]], we get:

$$Z_{MMSE} = \mu_Y + \rho\frac{\sigma_Y}{\sigma_X}(X - \mu_X)$$

This shows that the MMSE estimator is a linear combination of X and a constant term.

Step 3: Minimize MSE
To minimize the MSE, we differentiate it with respect to X and equate it to zero:

$$\frac{d}{dX}E[(Y - Z)^2] = 0$$

Solving for X, we get:

$$X = E[Y] + \rho\frac{\sigma_Y}{\sigma_X}(X - E[X])$$

This is known as the Wiener filter equation.

Step 4: Final Estimator
Substituting this value of X in our MMSE estimator equation, we get our final estimator as:

$$Z_{MMSE} = (1-\rho^2)\mu_Y + \rho\frac{\sigma_Y}{\sigma_X}Y + (1-\rho)\mu_X$$

## Conclusion

The Minimum Mean Square Estimator is a powerful tool in statistical signal processing that allows us to estimate unknown quantities with minimum error. It is based on minimizing the [[mean square error]] between the estimated value and the true value. The Orthogonality Principle plays a crucial role in deriving this estimator. 