#stats 

Bernoulli trials are a sequence of ***independent*** experiments with two possible outcomes: success (with probability $p$) and failure (with probability $1-p$). These trials are named after Jacob Bernoulli, who introduced them in his work on probability theory.

## Key Theorems

1. **Bernoulli Trial Theorem**: In a sequence of $n$ Bernoulli trials, the probability of exactly $k$ successes is given by the binomial distribution:

$$ P(X = k) = \binom{n}{k} p^k (1-p)^{n-k} $$

2. **Law of Large Numbers**: As the number of trials $n$ approaches infinity, the proportion of successes converges to the true probability $p$. Formally:

$$ \lim_{n \to \infty} P\left(\left|\frac{X}{n} - p\right| < \epsilon\right) = 1 $$

## Step-by-Step Example

Suppose we have a biased coin with a probability of heads $p = 0.6$. We want to find the probability of getting exactly 3 heads in 5 tosses.

Using the Bernoulli Trial Theorem, we have:

$$ P(X = 3) = \binom{5}{3} (0.6)^3 (0.4)^2 = 10 \times 0.216 \times 0.16 = 0.3456 $$

Therefore, the probability of getting exactly 3 heads in 5 tosses with a biased coin is approximately 0.3456.

By understanding Bernoulli trials and their applications, we can analyze various real-world scenarios involving binary outcomes and make informed decisions based on probabilities.