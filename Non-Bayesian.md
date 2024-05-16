

Non-[[Bayesian]] methods, also known as frequentist methods, are a class of statistical techniques that do not rely on the principles of Bayesian inference. Unlike Bayesian methods, which use prior knowledge and beliefs to update the probability of a hypothesis, non-Bayesian methods only consider the observed data to make inferences. This approach is based on the frequentist interpretation of probability, which defines it as the long-run relative frequency of an [[event]].

In case with $f_{Y|X}(y|x)$:
pick x that maximizes $f_{Y|X}(y|x)$
maximum likelihood

in case without:
pick x that makes the [[Forward Model]] fit the best
## The Frequentist Interpretation of Probability

The frequentist interpretation of probability states that the probability of an [[event]] is equal to its relative frequency in an infinite number of repeated trials. In other words, if we were to repeat an experiment an infinite number of times under identical conditions, the proportion of times that a particular outcome occurs would converge to its true probability.

This interpretation differs from the Bayesian view, where probability represents a degree of belief in a particular hypothesis. In frequentist statistics, probabilities are objective and do not depend on any prior knowledge or beliefs.

## Key Theorems

### Law of Large Numbers

The Law of Large Numbers is a fundamental theorem in frequentist statistics that states that as the number of observations increases, the sample mean converges to the population mean. Mathematically, it can be expressed as:

$$\lim_{n\to\infty} \frac{1}{n}\sum_{i=1}^{n} X_i = \mu$$

where $X_i$ are independent and identically distributed random variables with mean $\mu$.

### [[Central Limit Theorem]]

The [[Central Limit Theorem]] ([[Central Limit Theorem|CLT]]) is another important theorem in frequentist statistics that describes the behavior of sample means from any distribution. It states that as the sample size increases, the distribution of sample means approaches a normal distribution with mean equal to the population mean and standard deviation equal to $\frac{\sigma}{\sqrt{n}}$, where $\sigma$ is the population standard deviation. Mathematically, it can be expressed as:

$$\lim_{n\to\infty} P\left(\frac{\bar{X}-\mu}{\sigma/\sqrt{n}} \leq x \right) = \Phi(x)$$

where $\bar{X}$ is the sample mean and $\Phi(x)$ is the [[cumulative distribution function]] of a standard normal distribution.

## Non-Bayesian Inference

Non-Bayesian methods use the observed data to make inferences about a population parameter. This is done by constructing an estimator, which is a function of the data that estimates the value of the parameter. The most commonly used estimators are the sample mean and sample [[variance]], which are unbiased and consistent estimators.

### Maximum Likelihood Estimation

Maximum Likelihood Estimation (MLE) is a non-Bayesian method for estimating parameters. It involves finding the values of parameters that maximize the likelihood function, which measures how likely it is to observe the given data for a particular [[set]] of parameter values. Mathematically, MLE can be expressed as:

$$\hat{\theta}_{MLE} = \arg \max_{\theta} L(\theta | x_1,...,x_n)$$

where $\hat{\theta}_{MLE}$ is the maximum likelihood estimate of parameter $\theta$, $L(\theta | x_1,...,x_n)$ is the likelihood function, and $x_1,...,x_n$ are observed data points.

### Hypothesis Testing

Hypothesis testing is another important aspect of non-Bayesian inference. It involves making decisions about a population parameter based on sample data. The process usually involves setting up null and alternative hypotheses and calculating a test statistic from the data. If the test statistic falls within a critical region determined by a pre-specified significance level, the null hypothesis is rejected in favor of the alternative hypothesis.

## Example:
Suppose I flip an unfair coin 100 times. What is the maximum likelihood estimate of "heads" based on the number of heads observed?

observed 56 heads:
$\hat{p}=\frac{56}{100} = .56 \pm \sqrt{\frac{\sigma^2}{N}}$  




## Step-by-Step Example: Estimating a Population Mean

Suppose we want to estimate the average height of all adults in a particular city. We collect a random sample of 100 adults and measure their heights. The sample mean is 170 cm, and the sample standard deviation is 10 cm.

1. Define the parameter of interest: In this case, it is the population mean height, denoted by $\mu$.
2. Choose an appropriate estimator: The sample mean, denoted by $\bar{X}$, is an unbiased and consistent estimator for $\mu$.
3. Calculate the point estimate: The point estimate for $\mu$ is simply the sample mean, which in this case is 170 cm.
4. Calculate [[confidence interval]]: Using the [[Central Limit Theorem|CLT]], we can construct a [[confidence interval]] for $\mu$ with a desired level of confidence (e.g., 95%). For our example, we get a [[confidence interval]] of (165.5 cm, 174.5 cm).
5. Interpretation: We can be 95% confident that the true population mean height falls within this interval.

## Conclusion

Non-Bayesian methods provide a frequentist approach to statistical inference that does not rely on prior knowledge or beliefs. They are based on the frequentist interpretation of probability and involve constructing estimators and conducting hypothesis tests using observed data. While they have their limitations, non-Bayesian methods are widely used in various fields and provide valuable insights into population parameters.