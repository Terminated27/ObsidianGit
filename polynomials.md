#math
![[Pasted image 20231215164117.png]]

A polynomial is a mathematical expression consisting of variables, coefficients, and exponents. It is formed by combining these elements using addition, subtraction, multiplication, and exponentiation operations. Polynomials are widely used in various areas of mathematics and have numerous applications in science, engineering, and computer science.

## Definition

A polynomial is an expression of the form:

$$
P(x) = a_nx^n + a_{n-1}x^{n-1} + \ldots + a_1x^1 + a_0
$$

where $a_n, a_{n-1}, \ldots, a_1,$ and $a_0$ are constants called coefficients, $x$ is the variable, and $n$ is a non-negative integer called the degree of the polynomial. The coefficient $a_n$ must be non-zero.

## Degree of a Polynomial

The degree of a polynomial is determined by the highest [[power]] of the variable in the expression. For example:

- The polynomial $P(x) = 3x^2 - 2x + 5$ has degree 2 since the highest [[power]] of $x$ is 2.
- The polynomial $Q(x) = 4x^3 - x^2 + x - 7$ has degree 3 since the highest [[power]] of $x$ is 3.

## Operations on Polynomials

### Addition and Subtraction

Polynomials can be added or subtracted by combining like terms. Like terms have the same variable raised to the same [[power]]. For example:

$$
(3x^2 - 2x + 5) + (4x^2 - x + 3) = (3+4)x^2 + (-2+(-1))x + (5+3)
$$

Simplifying further gives:

$$
7x^2 - 3x + 8
$$

### Multiplication

To multiply two polynomials, we use the distributive property and combine like terms. For example:

$$
(3x^2 - 2x + 5)(4x - 1) = (3x^2)(4x) + (3x^2)(-1) + (-2x)(4x) + (-2x)(-1) + (5)(4x) + (5)(-1)
$$

Simplifying further gives:

$$
12x^3 - 3x^2 - 8x^2 + 2x + 20x - 5 = 12x^3 - 11x^2 + 22x - 5
$$

### Division

Polynomial division involves dividing one polynomial by another. The result is a quotient and possibly a remainder. Division of polynomials is beyond the scope of this note, but it is important to note that not all divisions result in exact quotients.

## Factorization of Polynomials

Factorization is the process of expressing a polynomial as a product of its factors. Factoring polynomials can help us find their roots or simplify complex expressions. There are various methods for factoring polynomials, including:

- Factoring out common factors.
- Using the difference of squares formula: $a^2 - b^2 = (a+b)(a-b)$.
- Using the [[quadratic formula]] for quadratic polynomials.

## Key Theorems

### Remainder Theorem

The Remainder Theorem states that if a polynomial $P(x)$ is divided by $(x-a)$, then the remainder is equal to $P(a)$. In other words:

$$
\text{If } P(x) \text{ is divided by } (x-a), \text{ then } P(x) = Q(x)(x-a) + P(a)
$$

where $Q(x)$ is the quotient.

### Factor Theorem

The Factor Theorem states that if a polynomial $P(x)$ evaluates to zero when $x=a$, then $(x-a)$ is a factor of $P(x)$. In other words:

$$
\text{If } P(a) = 0, \text{ then } (x-a) \text{ is a factor of } P(x)
$$

## Example

Let's consider the polynomial $P(x) = x^3 - 4x^2 + x - 6$. We will find its factors and roots.

By using synthetic division or long division, we find that $(x-2)$ is a factor of $P(x)$. Dividing $P(x)$ by $(x-2)$ gives us:

$$
\begin{align*}
&\phantom{\quad} x^2 - 2x + 3 \\
&\underline{- (x^3 - 4x^2 + x - 6)} \\
&\phantom{\quad} \quad \quad \quad \quad \quad \quad \quad \quad \quad \quad -2x^2 + 3 \\
&\phantom{\quad} \underline{- (-2x^3 + 4x^2 - 2x + 12)} \\
&\phantom{\quad} \phantom{\underline{-}} x^2 -5
\end{align*}
$$

Therefore, we have factored $P(x)$ as $(x-2)(x^2-5)$. Setting each factor equal to zero, we find that the roots are $x=2$, $x=\sqrt{5}$, and $x=-\sqrt{5}$.

## Conclusion

Polynomials are versatile mathematical expressions that play a crucial role in various areas of mathematics. Understanding their properties, operations, and factorization methods allows us to solve problems and analyze complex mathematical models. 