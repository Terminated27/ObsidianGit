#stats

In probability theory, multiple continuous random variables refer to a [[set]] of two or more random variables that take on continuous values. These random variables can be jointly distributed and are often used to model complex systems where multiple factors influence the outcome.

## Joint [[Probability Density Function]]

The joint [[probability density function]] (PDF) of two continuous random variables $X$ and $Y$ is denoted as $f_{XY}(x,y)$. It describes the likelihood of both $X$ and $Y$ taking on specific values within a given range. The joint PDF satisfies the following properties:

1. Non-negativity: $f_{XY}(x,y) \geq 0$
2. Normalization: $\int \int f_{XY}(x,y) \,dx\,dy = 1$
## [[Marginal Probability]] Density Function

The [[marginal probability]] density function of a single variable can be obtained by integrating the joint PDF over all possible values of the other variable. For example, the marginal PDF of $X$ is given by:

$$f_X(x) = \int f_{XY}(x,y) \,dy$$

Similarly, the marginal PDF of $Y$ is given by:

$$f_Y(y) = \int f_{XY}(x,y) \,dx$$
## [[Conditional Probability]] Density Function

The [[conditional probability]] density function describes the distribution of one variable given the value of another variable. For example, the conditional PDF of $Y$ given $X=x$ is defined as:

$$f_{Y|X}(y|x) = \frac{f_{XY}(x,y)}{f_X(x)}$$

## Independence of Random Variables

Two continuous random variables $X$ and $Y$ are independent if their joint PDF can be expressed as the product of their marginal PDFs:

$$f_{XY}(x,y) = f_X(x)f_Y(y)$$

## [[Covariance]] and [[Correlation]]

The [[covariance]] between two continuous random variables $X$ and $Y$ is defined as:
$$
\begin{align}
\text{Cov}(X,Y) &= E[(X - \mu_X)(Y - \mu_Y)]\\
\\
&=E[XY]-E[X]\times E[Y]
\end{align}
$$

where $\mu_X$ and $\mu_Y$ are the means of $X$ and $Y$, respectively.

The [[correlation]] coefficient between $X$ and $Y$, denoted by $\rho$, is defined as:

$$\rho = \frac{\text{Cov}(X,Y)}{\sigma_X\sigma_Y}$$

where $\sigma_X$ and $\sigma_Y$ are the standard deviations of $X$ and $Y$, respectively.

Overall, understanding multiple continuous random variables allows for a more comprehensive analysis of complex systems in various fields such as finance, engineering, and biology.

## Example

Let's consider an example involving two continuous random variables $X$ and $Y$ representing the height and weight of individuals in a population.

Suppose the joint [[probability density function]] of $X$ (height in meters) and $Y$ (weight in kilograms) is given by:

$$f_{XY}(x,y) = \frac{1}{2\pi}e^{-\frac{x^2+y^2}{2}}$$

This represents a bivariate normal distribution with mean 0 and variance 1 for both $X$ and $Y$. 

From this joint PDF, we can calculate the marginal PDFs of $X$ and $Y$:

$$f_X(x) = \int_{-\infty}^{\infty} \frac{1}{2\pi}e^{-\frac{x^2+y^2}{2}} \,dy$$

$$f_Y(y) = \int_{-\infty}^{\infty} \frac{1}{2\pi}e^{-\frac{x^2+y^2}{2}} \,dx$$

We can also calculate the conditional PDF of $Y$ given $X=x$ using the formula:

$$f_{Y|X}(y|x) = \frac{f_{XY}(x,y)}{f_X(x)}$$

Additionally, we can determine if $X$ and $Y$ are independent by checking if their joint PDF can be expressed as the product of their marginal PDFs.

Finally, we can calculate the [[covariance]] and [[correlation]] coefficient between $X$ and $Y to understand the relationship between height and weight in this population.

This example illustrates how multiple continuous random variables can be used to model real-world data and analyze relationships between different variables.