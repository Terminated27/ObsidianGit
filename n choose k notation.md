#stats 
# Binomial Coefficient (n choose k) Notation

The binomial coefficient, denoted as $\binom{n}{k}$ or "n choose k," represents the number of ways to choose k elements from a [[set]] of n elements without regard to the [[order]]. It is defined as:

$$\binom{n}{k} = \frac{n!}{k!(n-k)!}$$

where $n!$ denotes the factorial of n.

## Key Theorems and Definitions

1. **Symmetry Property**: $\binom{n}{k} = \binom{n}{n-k}$ for all integers n and k.

2. **Pascal's Identity**: $\binom{n}{k} = \binom{n-1}{k-1} + \binom{n-1}{k}$ for all integers n > 0 and 0 ≤ k ≤ n.

3. **Combinatorial Interpretation**: $\binom{n}{k}$ represents the number of ways to choose a [[subset]] of k elements from a [[set]] of n elements.

## Step-by-Step Example

Let's calculate $\binom{5}{2}$ using the formula:

$$\binom{5}{2} = \frac{5!}{2!(5-2)!}$$
$$= \frac{5*4*3*2*1}{(2*1)(3*2*1)}$$
$$= 10$$

Therefore, there are 10 ways to choose 2 elements from a [[set]] of 5 elements.

By understanding the binomial coefficient notation and its properties, we can efficiently solve combinatorial problems involving choosing subsets from a given [[set]].