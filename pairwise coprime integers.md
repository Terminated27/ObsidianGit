#computing 
In number theory, a [[set]] of integers is said to be pairwise [[coprime]] if every pair of integers in the [[set]] are [[coprime]], i.e., their greatest common divisor (GCD) is 1. This concept is important in various areas of mathematics, including cryptography and number theory.

## Theorem: 

Given a [[set]] of integers $a_1, a_2, ..., a_n$, the integers are pairwise [[coprime]] if and only if for any distinct $i,j \in \{1,2,...,n\}$, we have $\text{gcd}(a_i,a_j) = 1$.

## Example:

Consider the [[set]] of integers {6, 10, 15}. To show that these integers are pairwise [[coprime]], we need to verify that the GCD of every pair is 1.

- GCD(6,10) = 2
- GCD(6,15) = 3
- GCD(10,15) = 5

Since none of the pairs have a GCD other than 1, the [[set]] {6,10,15} is not pairwise [[coprime]].

## Definition:

A [[set]] of integers is said to be mutually [[coprime]] if every integer in the [[set]] is [[coprime]] with every other integer in the [[set]]. In other words, for any distinct $i,j \in \{1,2,...n\}$ where n is the size of the [[set]], $\text{gcd}(a_i,a_j) = 1$.

Pairwise coprimality is a weaker condition compared to mutual coprimality. For example, while {4,9} are pairwise [[coprime]] (GCD(4,9)=1), they are not mutually [[coprime]] as they share a common factor (GCD(4,9)=1).

Pairwise [[coprime]] integers play a crucial role in various mathematical applications and [[algorithms]] where ensuring relatively prime numbers are necessary for efficient computations and security measures.