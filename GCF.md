
In number theory, the **greatest common factor (GCF)** of two integers $a$ and $b$, denoted as $\text{GCF}(a,b)$, is the largest positive integer that divides both $a$ and $b$ without leaving a remainder.

## Key Theorems:

1. **[[Euclidean Algorithm]]**: The GCF of two integers $a$ and $b$ can be found using the [[Euclidean Algorithm]], which states:
$$\text{GCF}(a,b) = \text{GCF}(b, a \mod b)$$

2. **[[Fundamental Theorem of Arithmetic]]**: Every integer greater than 1 can be uniquely expressed as a product of prime numbers.

## Step-by-Step Example:

Let's find the GCF of 24 and 36 using the [[Euclidean Algorithm]]:

1. $\text{GCF}(24,36) = \text{GCF}(36, 24)$ (by [[Euclidean Algorithm]])
2. $\text{GCF}(36,24) = \text{GCF}(24, 12)$
3. $\text{GCF}(24,12) = \text{GCF}(12,0)$
4. Since the remainder is 0, we stop.
5. Therefore, $\text{GCF}(24,36) = 12$

By understanding the concepts of GCF and using tools like the [[Euclidean Algorithm]], we can efficiently find the greatest common factor of any two integers.