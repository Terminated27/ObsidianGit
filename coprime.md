#computing 

Coprime numbers, also known as relatively prime numbers, are integers that have no common factors other than 1. In other words, two numbers a and b are coprime if their greatest common divisor (GCD) is 1.

## Theorems:
1. **Euclid's Lemma**: If a prime number divides the product of two numbers, then it must divide at least one of the two numbers.
2. **[[Fundamental Theorem of Arithmetic]]**: Every integer greater than 1 can be expressed uniquely as a product of prime numbers (up to the order of the factors).

## Definition:
Two integers $a$ and $b$ are coprime if $\gcd(a,b) = 1$.

## Step-by-Step Example:
Let's consider two integers, $a = 15$ and $b = 28$. To determine if they are coprime, we calculate their GCD using Euclid's algorithm:

$$
\begin{align*}
\gcd(15,28) &= \gcd(28,15 \mod 28) \\
&= \gcd(28,15) \\
&= \gcd(15,28-15) \\
&= \gcd(15,13) \\
&= \gcd(13,15-13) \\
&= \gcd(13,2) \\
&= \gcd(2,1) \\
&= 1
\end{align*}
$$

Since $\gcd(15,28) = 1$, we conclude that 15 and 28 are coprime.

Coprime numbers play a crucial role in number theory and have applications in various mathematical problems such as cryptography and modular arithmetic. Understanding coprime integers helps in analyzing the properties of numbers and solving complex mathematical equations efficiently.