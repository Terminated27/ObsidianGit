

# Routh's Stability Criterion

Routh's Stability Criterion is a method used to determine the stability of a system based on the coefficients of its characteristic equation. It provides a necessary and sufficient condition for stability by analyzing the signs of the coefficients in the characteristic equation.

## Key Theorem
The key theorem in Routh's Stability Criterion states that for a system with a characteristic equation of the form:

$$
a_ns^n + a_{n-1}s^{n-1} + \ldots + a_1s + a_0 = 0
$$

The system is stable if and only if all coefficients $a_i$ are positive.

## Steps for Applying Routh's Stability Criterion

1. Write down the characteristic equation of the system.
2. Create a table with alternating rows starting with the coefficients of even powers of s and odd powers of s.
3. Fill in the first two rows with the coefficients of $s^n$ and $s^{n-2}$.
4. Calculate the remaining rows using the following formula:

$$
\begin{align*}
b_i &= \frac{a_{n-1}a_{n+1-i} - a_n a_{n-i}}{a_{n-1}} \\
\end{align*}
$$

5. Analyze the signs of the first column in the table. If all signs are positive, then the system is stable.

## Example

Consider a system with the characteristic equation:

$$
s^4 + 2s^3 + 3s^2 + 4s + 5 = 0
$$

Using Routh's Stability Criterion, we construct the table:

| s^4 | 1 | 3 |
|-----|---|---|
| s^2 | 2 | 4 |
| s^0 | b_1 | b_2 |

Calculating $b_1$ and $b_2$:

$$
\begin{align*}
b_1 &= \frac{2(4) - 1(3)}{2} = \frac{8 - 3}{2} = \frac{5}{2} > 0 \\
b_2 &= \frac{2b_1}{2} = \frac{5}{2} > 0 \\
\end{align*}
$$

Since all signs in the first column are positive, we can conclude that the system is stable based on Routh's Stability Criterion.