#diffeq #math 
In this atomic note, we will discuss the [[Laplace transform]] method for solving nonhomogeneous second-order ordinary differential equations (ODEs) with step functions. We will focus on providing additional insights and depth to the topic.

## Introduction

The [[Laplace transform]] is a powerful mathematical tool used to solve [[linear differential equations]]. It converts a [[Differential Equation]] into an algebraic equation, making it easier to solve. In this note, we will specifically look at how the [[Laplace transform]] can be applied to solve nonhomogeneous second-order ODEs that involve step functions.

## Theorem: [[Laplace Transform]] of a [[Step Function]]

Before diving into solving nonhomogeneous second-order ODEs, let's first state the theorem for the [[Laplace transform]] of a [[step function]].

**Theorem 1:** The [[Laplace transform]] of a [[step function]] $u(t-a)$ is given by:

$$
\mathcal{L}\{u(t-a)\} = \frac{e^{-as}}{s}, \quad s > 0
$$
$$
\mathcal{L}\{u(t-a)\} = \frac{e^{-s}}{s}, \quad s = 0
$$

where $a$ is a constant representing the time shift.

## Solving Nonhomogeneous Second-[[Order]] ODEs with Step Functions

Consider a nonhomogeneous second-[[order]] [[ODE]] in standard form:

$$y''(t) + p(t)y'(t) + q(t)y(t) = f(t), \quad t > 0$$

where $p(t)$ and $q(t)$ are continuous functions and $f(t)$ is a known function. We want to find the solution $y(t)$ that satisfies this equation.

To solve this [[ODE]] using the [[Laplace transform]] method, we follow these steps:

**Step 1:** Take the [[Laplace transform]] of both sides of the [[ODE]] with respect to $t$. Using linearity property of [[Laplace transform]], we have:

$$\mathcal{L}\{y''(t)\} + \mathcal{L}\{p(t)y'(t)\} + \mathcal{L}\{q(t)y(t)\} = \mathcal{L}\{f(t)\}$$

**Step 2:** Apply the [[Laplace transform]] formulas for derivatives and the [[Laplace transform]] of a [[step function]] (Theorem 1) to simplify the equation. This gives us:

$$s^2Y(s) - sy(0) - y'(0) + p(s)Y(s) - py(0) + q(s)Y(s) = F(s), \quad s > 0$$

where $Y(s)$ is the [[Laplace Transform]] of $y(t)$, $F(s)$ is the [[Laplace transform]] of $f(t)$, and $y(0)$ and $y'(0)$ are initial conditions.

**Step 3:** Rearrange the equation to solve for $Y(s)$:

$$(s^2 + p(s))Y(s) - (sy(0) + y'(0)) + (q(s)-p)y(0) = F(s), \quad s > 0$$

**Step 4:** Solve for $Y(s)$:

$$Y(s) = \frac{(sy(0)+y'(0)) - (q(s)-p)y(0)}{(s^2+p(s))} + \frac{F(s)}{(s^2+p(s))}, \quad s > 0$$

**Step 5:** Use [[partial fraction decomposition]] and [[inverse Laplace transform]] to find the solution $y(t)$.

To perform the [[partial fraction decomposition]], we need to factor the denominator of the second term in $Y(s)$:

$$s^3 + 3s^2 + 4 = (s+1)(s^2+2s+2)$$

The roots of $s^2+2s+2$ can be found using the [[quadratic formula]]:

$$s = \frac{-b \pm \sqrt{b^2-4ac}}{2a}$$

For $s^2+2s+2$, we have $a=1$, $b=2$, and $c=2$. Plugging these values into the [[quadratic formula]], we get:

$$s = \frac{-2 \pm \sqrt{(-2)^2-4(1)(2)}}{2(1)} = -1 \pm i$$

Therefore, the roots are complex conjugates: $s_1 = -1+i$ and $s_2 = -1-i$.

Now, let's perform the [[partial fraction decomposition]]. We write:

$$\frac{e^{-s}}{(s^3+3s^2+4)} = \frac{A}{(s+1)} + \frac{Bs+C}{(s^2+2s+2)}$$

Multiplying both sides by $(s^3 + 3s^2 + 4)$ and equating coefficients, we obtain:

$$e^{-s} = A(s^2 + 3) + (Bs+C)(s+1)$$

Expanding and collecting terms, we have:

$$e^{-s} = As^3 + (A+B)s^2 + (A+B+C)s + (A+C)$$

Comparing coefficients, we get the following system of equations:

$$A = 0$$
$$A + B = 0$$
$$A + B + C = 0$$
$$A + C = 1$$

From the first equation, we find $A=0$. Substituting this into the second equation, we get $B=0$. Substituting $A=0$ and $B=0$ into the third equation, we find $C=1$. Finally, substituting $A=0$ and $C=1$ into the fourth equation, we obtain $1+0=1$, which is true.

Therefore, the [[partial fraction decomposition]] is:

$$\frac{e^{-s}}{(s^3+3s^2+4)} = \frac{1}{(s^2+2s+2)}$$

Now, let's find the [[inverse Laplace transform]] of each term.

For the first term in $Y(s)$:

$$\frac{(sy(0)+y'(0))+(2y(0))}{(s^2+2s+2)} = \frac{s(y(0))+y'(0)+2(y(0))}{(s^2+2s+2)}$$

Using Theorem 5 from the [[Laplace Transform table]], we have:

$$\mathcal{L}^{-1}\left\{\frac{s}{(s^2+2s+2)}\right\} = e^{-t}\cos(t)$$

Applying Theorem 4 from the [[Laplace Transform table]] to find $\mathcal{L}^{-1}\left\{\frac{y'(0)+2(y(0))}{(s^2+2s+2)}\right\}$, we differentiate both sides with respect to $t$:

$$\mathcal{L}^{-1}\left\{\frac{y'(0)+2(y(0))}{(s^2+2s+2)}\right\} = \frac{d}{dt}\left(e^{-t}\cos(t)\right)$$

Using the [[Product Rule]] and the chain rule, we have:

$$\frac{d}{dt}\left(e^{-t}\cos(t)\right) = -e^{-t}\cos(t) + e^{-t}(-\sin(t)) = -e^{-t}(\cos(t)+\sin(t))$$

Therefore, the [[inverse Laplace transform]] of the first term is:

$$\mathcal{L}^{-1}\left\{\frac{(sy(0)+y'(0))+(2y(0))}{(s^2+2s+2)}\right\} = -e^{-t}(\cos(t)+\sin(t))$$

For the second term in $Y(s)$:

$$\frac{e^{-s}}{(s^3+3s^2+4)} = \frac{1}{(s^2+2s+2)}$$

Using Theorem 5 from the [[Laplace Transform table]], we have:

$$\mathcal{L}^{-1}\left\{\frac{1}{(s^2+2s+2)}\right\} = e^{-(t-1)} \sin((t-1))$$

Therefore, the [[inverse Laplace transform]] of the second term is:

$$\mathcal{L}^{-1}\left\{\frac{e^{-s}}{(s^3+3s^2+4)}\right\} = e^{-(t-1)} \sin((t-1))$$

Finally, adding both terms together, we get the solution $y(t)$:

$$y(t) = -e^{-t}(\cos(t)+\sin(t)) + e^{-(t-1)} \sin((t-1))$$

This is the solution to the [[nonhomogeneous second-order ODE]] with a [[step function]].## Example: Solving a [[Nonhomogeneous Second-Order ODE]] with a [[Step Function]]

Let's illustrate the above steps with an example. Consider the following nonhomogeneous second-order [[ODE]]:

$$y''(t) + 2y'(t) + 2y(t) = u(t-1), \quad t > 0$$

where $u(t)$ is the unit [[step function]].

**Step 1:** Taking the [[Laplace transform]] of both sides of the [[ODE]], we have:

$$s^2Y(s) - sy(0) - y'(0) + 2sY(s) - 2y(0) + 2Y(s) = \frac{e^{-s}}{s}, \quad s > 0$$

**Step 2:** Simplifying the equation using initial conditions and Theorem 1, we get:

$$(s^2 + 2s + 2)Y(s) - (sy(0) + y'(0)) - (2y(0)) = \frac{e^{-s}}{s}, \quad s > 0$$

**Step 3:** Rearranging the equation to solve for $Y(s)$, we obtain:

$$Y(s) = \frac{(sy(0)+y'(0))+(2y(0))}{(s^2+2s+2)} + \frac{e^{-s}}{(s^2+2s+2)s}, \quad s > 0$$

**Step 4:** Solving for $Y(s)$, we have:

$$Y(s) = \frac{(sy(0)+y'(0))+(2y(0))}{(s^2+2s+2)} + \frac{e^{-s}}{(s^3+3s^2+4)}, \quad s > 0$$

**Step 5:** Using [[partial fraction decomposition]] and inverse [[Laplace transform]], we find the solution $y(t)$.

## Conclusion

In this atomic note, we discussed the [[Laplace transform]] method for solving nonhomogeneous second-[[order]] ODEs with step functions. We provided a step-by-step approach and demonstrated an example to illustrate the process. The [[Laplace transform]] method is a powerful tool that allows us to convert differential equations into algebraic equations, making it easier to find solutions.