#stats 
A confidence interval is a range of values that is likely to contain the true value of a population parameter with a certain level of confidence. It is commonly used in statistics to estimate the unknown population parameter, such as the mean or proportion, based on a sample from the population.
## Formula

$$
\text{Confidence Interval} = \mu \pm z\frac{\sigma}{\sqrt{n}}
$$
where $\mu$ is mean
$z$ is confidence level value (in z score values)
$\sigma$ is standard deviation
$n$ is sample size


## Theorem: [[Central Limit Theorem]]

The [[central limit theorem]] states that if we have a random sample of size $n$ from a population with mean $\mu$ and standard deviation $\sigma$, then the sampling distribution of the sample mean $\bar{X}$ approaches a normal distribution as $n$ increases, regardless of the shape of the population distribution. This allows us to use normal distribution properties to make inferences about the population.

## Definition: Confidence Level

The confidence level is the probability that the true value of the population parameter falls within the calculated confidence interval. It is typically expressed as a percentage, such as 95% or 99%.

## Theorem: Margin of Error

The margin of error is defined as half the width of a confidence interval. It represents how much we can expect our estimate to vary from the true value in either direction. It is calculated using critical values from the normal distribution and depends on both the sample size and confidence level.
## Example:
estimate p=P(A) from data
$$
\hat{P} = \frac{\text{\# of outcomes of A}}{N} = \frac{1}{N}\Sigma^N_{i=1}x_i
$$
$$
\begin{align}
P(x=1)&=p \\
P(x=0)&=1-p
\end{align}
$$
Next we need to find $\sigma^2$ for $X$, we need to also find P
$$
Var(X_i) = p-p^2$$
$$(\hat{p}-2\sqrt{\frac{p-p^2}{N}},\hat{p}+2\sqrt{\frac{p-p^2}{N}})
$$
if we don't know p there are 2 approaches
$$
\begin{numcases}{\text{Where } p=\hat{p}}
(\hat{p}-2\sqrt{\frac{\hat{p}-\hat{p}^2}{N}},\hat{p}+2\sqrt{\frac{\hat{p}-\hat{p}^2}{N}})
\end{numcases}
$$
$$
\begin{numcases}{\text{Always True }}
\hat{p}-\sqrt{\frac{1}{N}},\hat{p}-\sqrt{\frac{1}{N},}
\end{numcases}
$$

## Example:

Suppose we want to estimate the average height of all students at a university. We take a random sample of 50 students and find that their average height is 170 cm with a standard deviation of 5 cm. We want to construct a 95% confidence interval for this estimate.

Step 1: Determine critical values

Since our sample size is large (n=50), we can use critical values from the standard normal distribution for our calculation. For a 95% confidence level, our critical values are -1.96 and 1.96.

Step 2: Calculate margin of error

Using our formula for margin of error, we have:

$$
\text{Margin of Error} = 1.96 \times \frac{5}{\sqrt{50}} = 1.38
$$

Step 3: Construct the confidence interval

Our confidence interval is given by:

$$
170 \pm 1.38 = (168.62, 171.38)
$$

This means that we are 95% confident that the true average height of all students at the university falls between 168.62 cm and 171.38 cm.

## Conclusion

In summary, a confidence interval is a range of values that is likely to contain the true value of a population parameter with a certain level of confidence. It is based on the [[central limit theorem]] and depends on the sample size and confidence level. Understanding how to calculate and interpret confidence intervals is crucial in making accurate statistical inferences about a population.
