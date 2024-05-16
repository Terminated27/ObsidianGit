#stats 

Binomial probabilities are a fundamental concept in probability theory, particularly in the context of repeated independent trials with only two possible outcomes. The binomial distribution describes the probability of obtaining a certain number of successes in a fixed number of trials.

## Binomial Distribution

The binomial distribution is characterized by two parameters: the number of trials $n$ and the probability of success on each trial $p$. The [[probability mass function]] ([[Probability Mass Function|PMF]]) of the binomial distribution is given by:

$$ P(X = k) = \binom{n}{k} p^k (1-p)^{n-k} $$

where $X$ is the [[random variable]] representing the number of successes, $\binom{n}{k}$ denotes the binomial coefficient, and $k$ ranges from 0 to $n$.

## Key Theorems

### Binomial Theorem
The binomial theorem states that for any positive integer $n$, we have:

$$ (a + b)^n = \sum_{k=0}^{n} \binom{n}{k} a^{n-k} b^k $$

This theorem is crucial for expanding binomial expressions and simplifying calculations involving binomials.

## Step-by-Step Example

Suppose we have a biased coin that lands on heads with probability $p = 0.6$. If we toss this coin 5 times, what is the probability of getting exactly 3 heads?

Using the binomial [[Probability Mass Function|PMF]] formula, we have:

$$ P(X = 3) = \binom{5}{3} (0.6)^3 (0.4)^2 $$

Calculating this expression gives:

$$ P(X = 3) = \frac{5!}{3!2!} (0.6)^3 (0.4)^2 = 10 \times 0.216 \times 0.16 = 0.3456 $$

Therefore, the probability of getting exactly 3 heads in 5 tosses of a biased coin with $p=0.6$ is approximately 0.3456.

By understanding the principles behind binomial probabilities and mastering their applications, one can efficiently analyze various scenarios involving repeated trials with binary outcomes.