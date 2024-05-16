#stats

A Gaussian [[random variable]], also known as a normal [[random variable]], is a [[continuous random variable]] that follows a Gaussian distribution. It is characterized by its mean $\mu$ and variance $\sigma^2$.
#### Shorthand notation
$X$~$N(\mu,\sigma^2)$
## [[Probability Density Function]] (PDF)

The [[probability density function]] of a Gaussian [[random variable]] $X$ is given by:

$$
f(x) = \frac{1}{\sqrt{2\pi\sigma^2}} e^{-\frac{(x-\mu)^2}{2\sigma^2}}
$$

where $-\infty < x < \infty$
### [[Cumulative Distribution Function]] (CDF)

Given that $X$ follows a normal distribution with mean $\mu$ and variance $\sigma^2$, we can express the [[cumulative distribution function]] (CDF) of $X$ as:

$P(z) = \frac{1}{2\pi} \sum_{-\infty}^{x} e^{\frac{-u^2}{2}} du$

The CDF of $X$ for $X \leq x$ can be written as:

$P(X \leq x) = \Phi\left(\frac{x - \mu}{\sigma}\right)$

$\Phi(z) = \frac{1}{\sqrt{2\pi}}\int_{-\infty}^{z}e^{-u^2/2}du$

For $X$~$N(0,1)$, we have $\mu = 0$ and $\sigma = 1$. Therefore,

$P(X \leq x) = \Phi(\frac{x-0}{1})$

$P(X \leq x) = \Phi(x)$
## Key Properties

1. **Symmetry**: The Gaussian distribution is symmetric around its mean $\mu$.
   
2. **68-95-99.7 Rule**: In a Gaussian distribution, approximately 68% of the values lie within one standard deviation ($\pm \sigma$) from the mean, 95% lie within two standard deviations ($\pm 2\sigma$), and 99.7% lie within three standard deviations ($\pm 3\sigma$).

3. **[[Central Limit Theorem]]**: The sum of a large number of independent and identically distributed random variables tends towards a Gaussian distribution.

4. **Mathematical properties:** $0\geq f_x(x)$ and integrates to $\int_{-\infty}^{\infty} f_x(x)dx = 1$, $E[x] = \mu$

5. **Linear Operation**:  If $X$ and $Y$ are independent Gaussian random variables, then a linear combination of them, $aX + bY$, is also Gaussian.


## Example 1

Suppose $X$ follows a Gaussian distribution with mean $\mu = 0$ and variance $\sigma^2 = 1$. Find the probability that $X$ lies between -1 and 1.

**Solution:**

We need to find $P(-1 < X < 1)$, which can be calculated using the [[cumulative distribution function]]:

$$
P(-1 < X < 1) = \int_{-1}^{1} f(x) dx
$$

Substitute the PDF $f(x)$ into the [[integral]]:

$$
P(-1 < X < 1) = \int_{-1}^{1} \frac{1}{\sqrt{2\pi}} e^{-x^2/2} dx
$$

This [[integral]] does not have a closed-form solution, but it can be approximated using the CDF

For $X$~$N(0,1)$, we have $\mu = 0$ and $\sigma = 1$. Therefore,

$\phi(X \leq x) = \Phi(\frac{x-0}{1})$

$\phi(X \leq x) = \Phi(x)$

So, for $X$~$N(0,1)$, the [[cumulative distribution function]] is simply $\Phi(x)$ where $\Phi(z)$ is the standard normal distribution function.
By understanding the properties and characteristics of Gaussian random variables, we can analyze various phenomena in statistics and probability theory with precision and accuracy.
## Example 2

Let's find the distribution of the [[random variable]] $Y = -3X + 2$, where $X$ follows a Gaussian distribution with mean $\mu = 1$ and variance $\sigma^2 = 4$.

Given that $X$ follows a normal distribution $X$~$N(1,4)$, we have $\mu = 1$ and $\sigma = 2$. 

To find the distribution of $Y$, we first calculate the mean and variance of $Y$:

Mean of Y:
$$
E[Y] = E[-3X + 2] = -3E[X] + 2 = -3(1) + 2 = -1
$$

Variance of Y: (the addition does not impact variance)
$$
Var(Y) = Var(-3X + 2) = (-3)^2 Var(X) = 9(4) = 36
$$

Therefore, the [[random variable]] $Y$ follows a Gaussian distribution with mean $\mu_Y = -1$ and variance $\sigma_Y^2 = 36$. In shorthand notation:

$Y$~$N(-1,36)$

This means that $Y$ is normally distributed with a mean of -1 and a standard deviation of 6.