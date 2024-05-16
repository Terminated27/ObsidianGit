#calc #math 

Partial fraction decomposition is a method used to express a rational function as the sum of simpler fractions. It is particularly useful when integrating rational functions or solving [[linear]] differential equations.

## Definition

Let $P(x)$ and $Q(x)$ be [[polynomials]] such that the degree of $P(x)$ is less than the degree of $Q(x)$. The partial fraction decomposition of $\frac{P(x)}{Q(x)}$ is given by:

$$\frac{P(x)}{Q(x)} = \sum_{i=1}^{n}\frac{A_i}{(x-a_i)^{m_i}}$$

where $a_i$ are distinct [[complex numbers]] and $m_i$ are positive integers.

## Theorem 1: [[Linear]] Factors

If $(x-a)$ is a [[linear]] factor of the polynomial $Q(x)$, then the partial fraction decomposition includes the term $\frac{A}{x-a}$, where $A$ is a constant.

## Theorem 2: Repeated [[Linear]] Factors

If $(x-a)^k$ is a repeated [[linear]] factor of the polynomial $Q(x)$, then the partial fraction decomposition includes terms $\frac{A_1}{x-a} + \frac{A_2}{(x-a)^2} + \ldots + \frac{A_k}{(x-a)^k}$, where $A_1, A_2, \ldots, A_k$ are constants.

## Theorem 3: Irreducible Quadratic Factors

If $(ax^2+bx+c)$ is an irreducible quadratic factor of the polynomial $Q(x)$, then the partial fraction decomposition includes the term $\frac{Ax+B}{ax^2+bx+c}$, where $A$ and $B$ are constants.


## Example 0 Cover up method

$$
\frac{x-7}{(x-1)(x+2)}
$$

To decompose $\frac{x-7}{(x-1)(x+2)}$ into partial fractions using the cover up method, we first write it as:
$$
\frac{x-7}{(x-1)(x+2)} = \frac{A}{x-1} + \frac{B}{x+2}
$$

Next, we multiply both sides by $(x-1)(x+2)$ to get rid of the denominators:
$$
x - 7 = A(x+2) + B(x-1)
$$

Now, we can use the cover up method to find the values of $A$ and $B$. To find $A$, we cover up the $(x-1)$ term and evaluate the equation at $x=1$:
$$
\begin{align}
1 - 7 &= A(1+2) + B(1-1) \\
-6 &= 3A \\
A &= -2
\end{align}
$$

To find $B$, we cover up the $(x+2)$ term and evaluate the equation at $x=-2$:
$$
\begin{align}
-2 - 7 &= A(-2+2) + B(-2-1) \\
-9 &= -3B \\
B &= 3
\end{align}
$$

Therefore, $\frac{x-7}{(x-1)(x+2)}$ can be decomposed into partial fractions as:
$$
\frac{x-7}{(x-1)(x+2)} = \frac{-2}{x-1} + \frac{3}{x+2}
$$


## Example 1

Find the partial fraction decomposition of $\frac{4x+1}{x^2-3x+2}$.

First, we factor the denominator as $(x-1)(x-2)$. Since we have distinct [[linear]] factors, we can use Theorem 1. Thus, the partial fraction decomposition is:

$$\frac{4x+1}{x^2-3x+2} = \frac{A}{x-1} + \frac{B}{x-2}$$

To find the values of $A$ and $B$, we can multiply both sides by the denominator and equate coefficients. This gives us:

$4x + 1 = A(x-2) + B(x-1)$

Expanding and collecting like terms, we get:

$4x + 1 = (A+B)x - (2A+B)$

Comparing coefficients, we have:

$A+B = 4$

$-2A-B = 1$

Solving this system of equations, we find $A=3$ and $B=1$. Therefore, the partial fraction decomposition is:

$$\frac{4x+1}{x^2-3x+2} = \frac{3}{x-1} + \frac{1}{x-2}$$

## Example 2:
Find the partial fraction decomposition of $\frac{3x^2+5x+1}{(x+1)(x^2+4)}$.

First, we factor the denominator as $(x+1)(x^2+4)$. Since we have a repeated [[linear]] factor, we can use Theorem 2. Thus, the partial fraction decomposition is:

$$\frac{3x^2+5x+1}{(x+1)(x^2+4)} = \frac{A}{x+1} + \frac{B}{x^2+4}$$

To find the values of $A$ and $B$, we can multiply both sides by the denominator and equate coefficients. This gives us:

$3x^2 + 5x + 1 = A(x^2 + 4) + B(x + 1)$

Expanding and collecting like terms, we get:

$3x^2 + 5x + 1 = (A+B)x^2 + Bx + (4A+B)$

Comparing coefficients, we have:

$A+B = 3$

$B = 5$

$4A+B = 1$

Solving this system of equations, we find $A=-\frac{11}{3}$ and $B=5$. Therefore, the partial fraction decomposition is:

$$\frac{3x^2+5x+1}{(x+1)(x^2+4)} = \frac{-\frac{11}{3}}{x+1} + \frac{5}{x^2+4}$$

## Example 3:
Find the partial fraction decomposition of $\frac{x-7}{(x-3)^3}$.

Since we have a repeated [[linear]] factor, we can use Theorem 2. Thus, the partial fraction decomposition is:

$$\frac{x-7}{(x-3)^3} = \frac{A}{x-3} + \frac{B}{(x-3)^2} + \frac{C}{(x-3)^3}$$

To find the values of $A$, $B$, and $C$, we can multiply both sides by the denominator and equate coefficients. This gives us:

$x - 7 = A(x-3)^2 + B(x-3) + C$

Expanding and collecting like terms, we get:

$x - 7 = (A)x^2 + (-6A+B)x + (9A-3B+C)$

Comparing coefficients, we have:

$A = 0$

$-6A+B = 1$

$9A-3B+C = -7$

Solving this system of equations, we find $A=0$, $B=1$, and $C=-7$. Therefore, the partial fraction decomposition is:

$$\frac{x-7}{(x-3)^3} = \frac{1}{(x-3)^2} - \frac{7}{(x-3)^3}$$
