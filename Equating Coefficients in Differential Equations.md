#diffeq #math 

In the study of differential equations, it is often necessary to solve for unknown coefficients that appear in the equations. One powerful method to achieve this is by equating coefficients. This technique allows us to determine the values of these coefficients by comparing the terms on both sides of the equation. In this atomic note, we will explore how to equate coefficients in differential equations and provide step-by-step examples.

## The Method of Equating Coefficients

The method of equating coefficients involves comparing the coefficients of like terms on both sides of a [[Differential Equation]]. By setting these coefficients equal to each other, we can obtain a system of equations that can be solved to find the unknown values.

Consider a general [[linear]] homogeneous [[ordinary differential equation]]:

$$
a_n(x)y^{(n)} + a_{n-1}(x)y^{(n-1)} + \ldots + a_1(x)y' + a_0(x)y = 0 \quad \text{(1)}
$$

where $y$ is an unknown function and $a_i(x)$ are known functions.

To solve for the unknown coefficients, we assume that $y$ can be expressed as a [[power series]]:

$$
y = c_0x^r + c_1x^{r+1} + c_2x^{r+2} + \ldots \quad \text{(2)}
$$

where $c_i$ are constants and $r$ is an arbitrary constant exponent. Substituting Equation (2) into Equation (1), we obtain:

$$
\begin{align*}
& a_n(x)(c_0x^r + c_1x^{r+1} + c_2x^{r+2} + \ldots)^{(n)} \\
&+ a_{n-1}(x)(c_0x^r + c_1x^{r+1} + c_2x^{r+2} + \ldots)^{(n-1)} \\
&+ \ldots \\
&+ a_1(x)(c_0x^r + c_1x^{r+1} + c_2x^{r+2} + \ldots)' \\
&+ a_0(x)(c_0x^r + c_1x^{r+1} + c_2x^{r+2} + \ldots) = 0
\end{align*}
$$

Expanding the derivatives and simplifying the equation, we can collect terms with the same powers of $x$. Equating the coefficients of these terms to zero, we obtain a [[set]] of equations that can be solved for the unknown coefficients $c_i$.

## Example: Solving a [[Differential Equation]] using Equating Coefficients

Let's illustrate the method of equating coefficients with an example. Consider the following second-[[order]] [[linear]] homogeneous [[ordinary differential equation]]:

$$
y'' - 3xy' - x^2y = 0 \quad \text{(3)}
$$

To solve this equation, we assume that $y$ can be expressed as a [[power series]]:

$$
y = c_0 + c_1x + c_2x^2 + \ldots \quad \text{(4)}
$$

Substituting Equation (4) into Equation (3), we obtain:

$$
\begin{align*}
&(c_2 - 6c_3)x^0 \\
&+(6c_3 - 12c_4 - 6c_2)x^1 \\
&+(12c_4 - 20c5 - 3c2)x^2 \\
&+(20c5 - 30c6 - c4)x^3 \\
&+ \ldots = 0
\end{align*}
$$

Equating the coefficients of like powers of $x$ to zero, we have:

$$
\begin{align*}
c_2 - 6c_3 &= 0 \quad \text{(5)} \\
6c_3 - 12c_4 - 6c_2 &= 0 \quad \text{(6)} \\
12c_4 - 20c5 - 3c2 &= 0 \quad \text{(7)} \\
20c5 - 30c6 - c4 &= 0 \quad \text{(8)} \\
&\vdots
\end{align*}
$$

Solving this system of equations will yield the values of the unknown coefficients $c_i$, allowing us to determine the solution to the original [[Differential Equation]].

## Conclusion

The method of equating coefficients is a powerful technique for solving differential equations. By comparing the coefficients of like terms on both sides of an equation, we can obtain a system of equations that can be solved for