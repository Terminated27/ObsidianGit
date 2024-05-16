

Hurwitz's Stability Criterion is a method used to determine the stability of a polynomial system by analyzing the coefficients of its [[characteristic equation]]. The criterion states that a polynomial system is stable if and only if all the coefficients of its [[characteristic equation]] are positive.

## Theorem

Let $P(s) = a_ns^n + a_{n-1}s^{n-1} + \ldots + a_1s + a_0$ be a polynomial with real coefficients. The system described by $P(s)$ is stable if and only if:

1. $a_n > 0$
2. $a_{n-1} > 0$
3. $\ldots$
4. $a_0 > 0$

## Example

Consider the [[characteristic equation]] of a system given by:

$$P(s) = s^3 + 2s^2 + 3s + 4$$

To apply Hurwitz's Criterion, we need to check if all coefficients are positive:

1. $a_3 = 1 > 0$
2. $a_2 = 2 > 0$
3. $a_1 = 3 > 0$
4. $a_0 = 4 > 0$

Since all coefficients are positive, the system described by $P(s)$ is stable according to Hurwitz's Stability Criterion.

By using Hurwitz's Stability Criterion, engineers can quickly assess the stability of systems without having to solve for [[Eigenvalues]] or perform complex calculations, making it a valuable tool in control theory and system analysis.