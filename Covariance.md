Covariance is a measure of the linear relationship between two random variables. It measures how much two variables change together, or in other words, how much they vary together.

## Definition

The covariance between two random variables X and Y is defined as:
	
$$
\begin{align}
\text{Cov}(X,Y) &= E[(X - \mu_X)(Y - \mu_Y)]\\
\\
&=E[XY]-E[X]\times E[Y]
\end{align}
$$

where $\mu_X$ and $\mu_Y$ are the means of X and Y respectively.

## Properties

1. Covariance is symmetric: $\text{Cov}(X,Y) = \text{Cov}(Y,X)$
2. If X and Y are independent, then their covariance is 0: $\text{Cov}(X,Y) = 0$
3. If X and Y have a perfect positive linear relationship, then their covariance is equal to the product of their standard deviations: $\text{Cov}(X,Y) = \sigma_X\sigma_Y$
4. If X and Y have a perfect negative linear relationship, then their covariance is equal to the negative product of their standard deviations: $\text{Cov}(X,Y) = -\sigma_X\sigma_Y$

## Interpretation

The sign of covariance indicates the direction of the linear relationship between two variables. A positive covariance means that when one variable increases, the other tends to increase as well. A negative covariance means that when one variable increases, the other tends to decrease.

The magnitude of covariance indicates the strength of the linear relationship between two variables. A larger magnitude indicates a stronger linear relationship, while a smaller magnitude indicates a weaker linear relationship.

However, it should be noted that covariance alone does not provide information about the strength or direction of [[non-linear]] relationships between variables.

## Calculation

To calculate covariance between two random variables X and Y from a sample data [[set]] with n observations, we can use the following formula:

$$
\text{Cov}(X,Y) = \frac{\sum_{i=1}^{n}(x_i - \bar{x})(y_i - \bar{y})}{n-1}
$$

where $x_i$ and $y_i$ are the individual observations of X and Y, and $\bar{x}$ and $\bar{y}$ are the sample means of X and Y respectively.

## Example

Consider a data [[set]] with 5 observations for two variables X and Y:

| X | Y |
|---|---|
| 1 | 2 |
| 3 | 4 |
| 5 | 6 |
| 7 | 8 |
| 9 | 10 |

Step 1: Calculate the mean of X and Y.

$\bar{x} = \frac{1+3+5+7+9}{5} = 5$

$\bar{y} = \frac{2+4+6+8+10}{5} = 6$

Step 2: Calculate the deviations from the mean for each observation.

| x - $\bar{x}$ | y - $\bar{y}$ |
| ------------- | ------------- |
| -4            | -4            |
| -2            | -2            |
| 0             | 0             |
| 2             | 2             |
| 4             | 4             |

Step 3: Multiply the deviations for each observation.

| $x - \bar{x}$ | $y - \bar{y}$ |
| ------------- | ------------- |
| -4 x -4       | -16           |
| -2 x -2       | -4            |
| 0 x 0         | =0            |
| 2 x +2        | =4            |
| 4 x +4        | =16           |

Step 4: Sum up all the products.

$\sum_{i=1}^{n}(x_i - \bar{x})(y_i - \bar{y}) = (-16)+(-4)+0+4+16 = 0$

Step 5: Divide by n-1.

$\text{Cov}(X,Y) = \frac{0}{5-1} = 0$

Since the covariance is 0, we can conclude that there is no linear relationship between X and Y in this data [[set]].