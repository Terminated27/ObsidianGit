---
aliases:
  - CLT
---

The Central Limit Theorem (CLT) is a fundamental result in probability theory that describes the behavior of the sample mean of a large number of independent and identically distributed (i.i.d.) random variables. It states that under certain conditions, the sample mean will be approximately normally distributed, regardless of the underlying distribution of the individual random variables.

## Theorem Statement

Let $X_1, X_2, ..., X_n$ be a sequence of i.i.d. random variables with mean $\mu$ and [[variance]] $\sigma^2$. Then, as $n$ approaches infinity, the distribution of the sample mean $\bar{X}$ approaches a normal distribution with mean $\mu$ and [[variance]] $\frac{\sigma^2}{n}$.

$$\lim_{n \to \infty} P(\bar{X} \leq x) = \Phi\left(\frac{x-\mu}{\frac{\sigma}{\sqrt{n}}}\right)$$

where $\Phi(z)$ is the [[cumulative distribution function]] (CDF) of a standard normal distribution.
1. **Mean (Expected Value)**:
    - The mean $\mu$ for a binomial distribution is given by: $\mu = np$ where:
        - $n$ is the number of trials
        - $p$ is the probability of success.
    
2. **Variance**:
    - The variance $\sigma^2$ for a binomial distribution is calculated as: $\sigma^2 = npq$ where:
        - $q = 1 - p$ (probability of failure).
    
3. **Standard Deviation**:
    
    - The standard deviation $\sigma$ is the square root of the variance: $\sigma = \sqrt{\sigma^2}$
## Intuition

The CLT can be understood intuitively by considering the [[Law of Large Numbers]]. This law states that as we increase the sample size, the sample mean will converge to the true population mean. However, it does not specify how fast this convergence occurs or what is the shape of this convergence. The CLT provides an answer to these questions by stating that as $n$ increases, the distribution of $\bar{X}$ becomes more and more similar to a normal distribution.


**Central Limit Theorem Formula**:
  
- The CLT provides insights into the shape of the sampling distribution of the mean.
- We can describe this distribution using the following notation:
    - (X̄) represents the **sampling distribution of the sample means**.
    - The symbol “~” means “follows the distribution.”
    - (N) refers to the **normal distribution**.
-  The parameters of the sampling distribution of the mean are determined by the population parameters:
    - The **mean of the sampling distribution** $\mu_{\bar{X}}$ is equal to the **mean of the population** $\mu$.
    -  The **standard deviation of the sampling distribution** $\sigma_{\bar{X}}$ is calculated as: $$ \sigma_{\bar{X}} = \frac{\sigma}{\sqrt{n}} $$ where:
        - $\sigma$ is the **standard deviation of the population**.
        - $n$ is the **sample size**.
**Example**:
    
- Suppose we have a population with a mean age of 34 years and a standard deviation of 15 years.
- If we take random samples of size 50, the standard deviation of the sampling distribution of the mean would be: $\sigma_{\bar{X}} = \frac{15}{\sqrt{50}}$