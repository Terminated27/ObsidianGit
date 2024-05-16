
Variance is a measure of how spread out a [[set]] of data is. It is commonly used in statistics and probability to quantify the variability or dispersion of a [[random variable]] or a [[set]] of data points.
usually represented as $\sigma^2$
## Definition

The variance of a [[random variable]] measures how spread out its values are around the mean. It is defined as:

$$
Var(X) = E[(X - E[X])^2]
$$
or
$$
Var(X) = E[X^2] - E[X]^2
$$
and the standard deviation is the square root of the variance.

## Properties

1. The variance is always non-negative: $\operatorname{Var}(X) \geq 0$
2. If all values in the data [[set]] are equal, then the variance is zero.
3. The units of variance are squared units of the original data.
4. The variance of a constant value is zero: $\operatorname{Var}(c) = 0$
5. For any constant $c$, $\operatorname{Var}(cX) = c^2\operatorname{Var}(X)$

## Calculating Variance

To calculate the variance, we first need to find the mean ($\mu$) and then follow these steps:

1. Subtract the mean from each data point: $(x_i - \mu)$
2. Square each difference: $(x_i - \mu)^2$
3. Find the average of these squared differences by summing them up and dividing by the total number of data points: $\frac{\sum_{i=1}^{n}(x_i - \mu)^2}{n}$
4. This average is the variance: $\operatorname{Var}(X) = \frac{\sum_{i=1}^{n}(x_i - \mu)^2}{n}$

## Theorem: Chebyshev's Inequality

Chebyshev's inequality provides an upper bound for the probability that a [[random variable]] deviates from its mean by more than a certain amount.

For any [[random variable]] $X$ with mean $\mu$ and variance $\sigma^2$, and any constant $k > 0$, the following holds:

$$
P(|X - \mu| \geq k\sigma) \leq \frac{1}{k^2}
$$

## Example

Suppose we have a data [[set]] of exam scores for a class with the following values: 70, 75, 80, 85, and 90. To calculate the variance, we first find the mean:

$$
\mu = \frac{70 + 75 + 80 + 85 + 90}{5} = 80
$$

Then, we subtract the mean from each data point and square it:

$(70 - 80)^2 = (-10)^2 = 100$

$(75 - 80)^2 = (-5)^2 =25$

$(80 - 80)^2 = (0)^2 =0$

$(85 - 80)^2 = (5)^2 =25$

$(90 - 80)^2 = (10)^2 =100$

Next, we find the average of these squared differences:

$\frac{100+25+0+25+100}{5}=\frac{250}{5}=50$

Therefore, the variance of this data [[set]] is $\operatorname{Var}(X) =50$. This means that on average, each data point deviates from the mean by 50 units squared.

## Conclusion

Variance is a useful tool in statistics and probability to measure the spread of data. It provides valuable insights into the variability of a [[random variable]] or a [[set]] of data points. Chebyshev's inequality also allows us to make probabilistic statements about how much a [[random variable]] deviates from its mean. By understanding and calculating variance, we can better understand and analyze data sets.