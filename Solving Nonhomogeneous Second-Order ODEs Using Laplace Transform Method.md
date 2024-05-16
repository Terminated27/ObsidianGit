#diffeq 

In this atomic note, we will explore the [[Laplace transform]] method for solving nonhomogeneous second-order ordinary differential equations (ODEs). We will focus on equations of the form:

$$
y''(t) + p(t)y'(t) + q(t)y(t) = g(t)
$$

where $p(t)$, $q(t)$, and $g(t)$ are given functions.

## Theorem 1: [[Laplace Transform]] of Derivatives

Let $f(t)$ be a function with [[Laplace transform]] $F(s)$. Then the [[Laplace transform]] of its [[Derivative]] $\frac{d}{dt}f(t)$ is given by:

$$
\mathcal{L}\left\{\frac{d}{dt}f(t)\right\} = sF(s) - f(0)
$$

## Theorem 2: Initial Value Theorem

If $f(t)$ is a function with [[Laplace transform]] $F(s)$ and $\lim_{{t \to 0}} f(t) = L$, then:

$$
\lim_{{s \to \infty}} sF(s) = L
$$

## Theorem 3: [[Convolution]] Theorem

If $F(s)$ and $G(s)$ are the Laplace transforms of functions $f(t)$ and $g(t)$ respectively, then the [[Laplace transform]] of their [[convolution]] $(f * g)(t)$ is given by:

$$
\mathcal{L}\{(f * g)(t)\} = F(s)G(s)
$$

## Step-by-Step Example: Solving a [[Nonhomogeneous Second-Order ODE]] using [[Laplace Transform]] Method

**Example:** Solve the following [[nonhomogeneous second-order ODE]] using the [[Laplace transform]] method:

$$
y''(t) + 2y'(t) + 2y(t) = e^{-t}
$$

**Step 1:** Take the [[Laplace transform]] of both sides of the equation. Using Theorem 1, we have:

$$
s^2Y(s) - sy(0) - y'(0) + 2sY(s) - 2y(0) + 2Y(s) = \frac{1}{s+1}
$$

where $Y(s)$ is the [[Laplace transform]] of $y(t)$.

**Step 2:** Rearrange the equation to solve for $Y(s)$:

$$
(Y(s))(s^2 + 2s + 2) - sy(0) - y'(0) - 2y(0) = \frac{1}{s+1}
$$

**Step 3:** Substitute initial conditions $y(0)$ and $y'(0)$ into the equation. Let's assume $y(0)=a$ and $y'(0)=b$:

$$
(Y(s))(s^2 + 2s + 2) - sa - b - 2a = \frac{1}{s+1}
$$

**Step 4:** Solve for $Y(s)$:

$$
(Y(s))(s^2 + 3s + 2) = \frac{1}{s+1} + (3a+b)
$$

Dividing both sides by $(s^2 + 3s + 2)$, we get:

$$
Y(s) = \frac{1}{(s+1)(s^2+3s+2)} + \frac{(3a+b)}{(s^2+3s+2)}
$$

**Step 5:** Decompose the fraction on the right-hand side into partial fractions:

$$
Y(s) = \frac{A}{s+1} + \frac{B}{s+2} + \frac{C}{s+1}
$$

where $A$, $B$, and $C$ are constants to be determined.

**Step 6:** Solve for the constants $A$, $B$, and $C$. Multiplying both sides by the common denominator $(s+1)(s+2)$, we have:

$$
A(s+2) + B(s+1) + C(s^2+s) = 1 + (3a+b)(s^2+s)
$$

Comparing coefficients of like powers of $s$, we get the following system of equations:
$$
\begin{align*}
A + B + C &= 1 \\
2A + B &= (3a+b)
\end{align*}
$$
Solving this system, we find $A = -\frac{b}{3}$, $B = a+b+\frac{b}{3}$, and $C = \frac{4b}{3}$.

**Step 7:** Substitute the values of the constants back into the equation for $Y(s)$:

$$
Y(s) = -\frac{b}{3}\left(\frac{1}{s+1}\right) + \left(a+b+\frac{b}{3}\right)\left(\frac{1}{s+2}\right) + \frac{4b}{3}\left(\frac{s}{s^2+s+2}\right)
$$

**Step 8:** Take the [[inverse Laplace transform]] of $Y(s)$ to obtain the solution in the time domain. Using table entries or [[Laplace transform]] properties, we find:
$$
\begin{align*}
y(t) &= -\frac{b}{3}e^{-t} + \left(a+b+\frac{b}{3}\right)e^{-2t} + \frac{4b}{3}\sin(t)
\end{align*}
$$
Therefore, the solution to the given [[nonhomogeneous second-order ODE]] is:

$$
y(t) = -\frac{b}{3}e^{-t} + \left(a+b+\frac{b}{3}\right)e^{-2t} + \frac{4b}{3}\sin(t)
$$

where $a$ and $b$ are the initial conditions $y(0)$ and $y'(0)$ respectively.

This concludes our discussion on solving nonhomogeneous second-order ODEs using the [[Laplace transform]] method.