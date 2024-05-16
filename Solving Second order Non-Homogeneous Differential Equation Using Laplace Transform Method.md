#diffeq #math 

The [[Laplace transform]] is a powerful tool used to solve differential equations by transforming them from the time domain to the frequency domain. In this atomic note, we will focus on finding the [[Laplace transform]] of second-order non-homogeneous differential equations.

## Definition

A second-order non-homogeneous [[linear differential]] equation can be written in the form:

$$
\frac{{d^2y}}{{dt^2}} + a_1 \frac{{dy}}{{dt}} + a_0y = f(t)
$$

where $a_1$ and $a_0$ are constants, and $f(t)$ is a known function.

## Theorem 1: Linearity Property of [[Laplace Transform]]

The [[Laplace transform]] has a linearity property that states:

$$
\mathcal{L}\{af(t) + bg(t)\} = aF(s) + bG(s)
$$

where $\mathcal{L}\{f(t)\} = F(s)$ and $\mathcal{L}\{g(t)\} = G(s)$.

## Theorem 2: [[Derivative]] Property of [[Laplace Transform]]

The [[derivative]] property of the [[Laplace transform]] states:

$$
\mathcal{L}\{\frac{{d^n f}}{{dt^n}}\} = s^nF(s) - s^{n-1}f(0) - s^{n-2}f'(0) - \ldots - f^{(n-1)}(0)
$$

where $\mathcal{L}\{f(t)\} = F(s)$.

## Step-by-Step Example

Let's consider the following second-order non-homogeneous differential equation:

$$
\frac{{d^2y}}{{dt^2}} + 3\frac{{dy}}{{dt}} + 2y = 2e^{-t} + 3\cos(t)
$$

To find the [[Laplace transform]] of this equation, we will follow these steps:

### Step 1: Take the [[Laplace transform]] of both sides

Applying the [[Laplace transform]] to both sides of the equation, we get:

$$
s^2Y(s) - sy(0) - y'(0) + 3sY(s) - 3y(0) + 2Y(s) = \frac{2}{s+1} + \frac{3}{s^2+1}
$$

To expand on this step, let's break down the [[Laplace transform]] of each term on the left side of the equation:

1. The [[Laplace transform]] of $y''(t)$ is $s^2Y(s)$.
2. The [[Laplace transform]] of $y'(t)$ is $sY(s) - y(0)$, where $y(0)$ represents the [[initial condition]] of the first [[derivative]].
3. The [[Laplace transform]] of $y(t)$ is $Y(s)$.
4. The [[Laplace transform]] of the constant term 3 is simply 3.

Therefore, applying the [[Laplace transform]] to both sides of the [[differential equation]] gives us:

$$
s^2Y(s) - sy(0) - y'(0) + 3sY(s) - 3y(0) + 2Y(s) = \frac{2}{s+1} + \frac{3}{s^2+1}
$$

Note that we have used linearity property of Laplace transforms to separate each term and applied the initial conditions for $y(t)$ and its [[derivative]] in terms of their Laplace transforms.

This step essentially converts the original [[differential equation]] into an algebraic equation in terms of the transformed variable $Y(s)$. We can now solve this algebraic equation to find the expression for $Y(s)$.

### Step 2: Simplify the equation

Rearranging terms and simplifying, we obtain:

$$
(Y(s)(s^2 + 3s + 2)) - (sy(0) + y'(0) + 3y(0)) = \frac{2}{s+1} + \frac{3}{s^2+1}
$$

### Step 3: Solve for Y(s)

Isolating $Y(s)$, we have:

$$
Y(s)(s^2 + 3s + 2) = \frac{2}{s+1} + \frac{3}{s^2+1} + sy(0) + y'(0) + (3y(0))
$$

Simplifying further:

$$
Y(s)(s^2 + 3s + 2) = \frac{2}{s+1} + \frac{3}{(s+i)(s-i)} + sy(0) + y'(0) + (3y(0))
$$

### Step 4: [[Partial fraction decomposition]]

We can decompose the term $\frac{3}{(s+i)(s-i)}$ into partial fractions as follows:

$$
\frac{3}{(s+i)(s-i)} = \frac{A}{s+i} + \frac{B}{s-i}
$$

Multiplying both sides by $(s+i)(s-i)$:

$$
3 = A(s-i) + B(s+i)
$$

Expanding and equating coefficients:

$$
3 = (A+B)s + (-Ai+Bi)
$$

Comparing the coefficients, we find $A=B=\frac{3}{2i}$.

Therefore, the [[partial fraction decomposition]] is:

$$
\frac{3}{(s+i)(s-i)} = \frac{\frac{3}{2i}}{s+i} + \frac{\frac{3}{2i}}{s-i}
$$

### Step 5: [[Inverse Laplace transform]]

Taking the [[inverse Laplace transform]] of both sides, we get:

$$
Y(s) = \mathcal{L}^{-1}\left\{\frac{2}{s+1}\right\} + \mathcal{L}^{-1}\left\{\frac{\frac{3}{2i}}{s+i}\right\} + \mathcal{L}^{-1}\left\{\frac{\frac{3}{2i}}{s-i}\right\} + y(0)s + y'(0) + 3y(0)
$$

Using the properties of [[Laplace transform]] and [[inverse Laplace transform]], we can simplify further to obtain the solution $y(t)$.

## Conclusion

In this atomic note, we discussed the [[Laplace transform]] of second-order non-homogeneous differential equations. We provided a step-by-step example to illustrate how to find the [[Laplace transform]] of such equations. The key theorems of linearity and [[derivative]] property were also included. The [[Laplace transform]] is a powerful tool that allows us to solve differential equations in the frequency domain, providing a different perspective on the behavior of systems.