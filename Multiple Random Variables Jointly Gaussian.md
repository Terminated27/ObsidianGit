#stats 

In probability theory, [[multiple random variables]] are said to be jointly Gaussian if their joint probability distribution is a multivariate normal distribution. This implies that any linear combination of the random variables is also normally distributed.

## Key Theorems:

1. **Characterization Theorem**: If random variables $X_1, X_2, \ldots, X_n$ are jointly Gaussian, then any linear combination of them $Y = a_1X_1 + a_2X_2 + \ldots + a_nX_n$ is also Gaussian.

$$Y \sim \mathcal{N}(\boldsymbol{\mu}_Y, \boldsymbol{\Sigma}_Y)$$

where $\boldsymbol{\mu}_Y = [a_1, a_2, \ldots, a_n] \begin{bmatrix} \mu_{X_1} \\ \mu_{X_2} \\ \vdots \\ \mu_{X_n} \end{bmatrix}$ and $\boldsymbol{\Sigma}_Y = [a_i a_j]_{n\times n}[\Sigma_{ij}]_{n\times n}$.

2. **Independence and Joint Gaussianity**: If [[multiple random variables]] are jointly Gaussian and independent, then they are also uncorrelated.

The expected value of a linear combination of jointly Gaussian random variables can be calculated using the linearity of expectation. 

If $Y = a_1X_1 + a_2X_2 + \ldots + a_nX_n$ is a linear combination of jointly Gaussian random variables, then the expected value of $Y$ is given by:

$$E[Y] = E[a_1X_1 + a_2X_2 + \ldots + a_nX_n]$$

Since expectation is a linear operator, we can distribute it over the sum:

$$E[Y] = a_1E[X_1] + a_2E[X_2] + \ldots + a_nE[X_n]$$

Using the properties of jointly Gaussian random variables, we know that each $X_i$ has an expected value $\mu_{X_i}$, so:

$$E[Y] = a_1\mu_{X_1} + a_2\mu_{X_2} + \ldots + a_n\mu_{X_n}$$

Therefore, the expected value of the linear combination $Y$ is simply the weighted sum of the [[expected values]] of the individual random variables.
## Step-by-Step Example:

Consider two jointly Gaussian random variables $X$ and $Y$ with means $\mu_X$, $\mu_Y$, variances $\sigma_X^2$, $\sigma_Y^2$, and [[correlation]] coefficient $\rho$. The joint PDF of $X$ and $Y$ is given by:

$$f_{XY}(x,y) = \frac{1}{2\pi\sigma_X\sigma_Y\sqrt{1-\rho^2}}\exp\left(-\frac{1}{2(1-\rho^2)}\left[\frac{(x-\mu_X)^2}{\sigma_X^2}- 2\rho\frac{(x-\mu_X)(y-\mu_Y)}{\sigma_X\sigma_Y}+\frac{(y-\mu_Y)^2}{\sigma_Y^2}\right]\right)$$

To find the conditional distribution of $X$ given $Y=y$, we use the conditional PDF formula for jointly Gaussian random variables:

$$f_{X|Y}(x|y) = \frac{f_{XY}(x,y)}{f_Y(y)}$$

where $f_Y(y)$ is the marginal PDF of $Y$. Substituting the expressions for $f_{XY}(x,y)$ and $f_Y(y)$ into the above equation gives us the conditional distribution of $X$ given $Y=y$.