#diffeq 

Differential equations are mathematical equations that describe the relationship between a function and its derivatives. They are used to model a wide range of phenomena in various fields such as physics, engineering, economics, and biology. In this atomic note, we will discuss the basics of differential equations, including key theorems, definitions, and step-by-step examples.

## Types of Differential Equations

There are several types of differential equations based on their [[order]] and type of variables. The most common types are:

- **Ordinary Differential Equations (ODEs)**: These equations involve only one independent variable and its derivatives with respect to that variable.
- **Partial Differential Equations (PDEs)**: These equations involve multiple independent variables and their partial derivatives.
- **[[Linear Differential Equations]]**: These equations have [[linear]] terms in the dependent variable and its derivatives.
- **Nonlinear Differential Equations**: These equations have nonlinear terms in the dependent variable and its derivatives.

In this note, we will focus on ODEs as they are more commonly used in applications.

## Notation

The general form of an [[ODE]] is given by:

$$F(x,y,y',y'',...,y^{(n)}) = 0$$

where $x$ is the independent variable, $y$ is the dependent variable, $y'$ is the first [[derivative]] of $y$, $y''$ is the second [[derivative]] of $y$, and so on until $y^{(n)}$ which represents the nth [[derivative]] of $y$. The [[order]] of an [[ODE]] is determined by the highest [[derivative]] present in the equation.

## Initial Value Problem (IVP)

An initial value problem (IVP) is a type of boundary value problem where we are given both an [[ODE]] and initial conditions for the dependent variable at a specific point. The general form of an IVP is given by:

$$F(x,y,y',y'',...,y^{(n)}) = 0, \quad y(x_0) = y_0, \quad y'(x_0) = y'_0, \quad ..., \quad y^{(n-1)}(x_0) = y^{(n-1)}_0$$

where $x_0$ is the initial value of the independent variable and $y_0, y'_0, ..., y^{(n-1)}_0$ are the initial values of the dependent variable and its derivatives.

## [[Existence and Uniqueness Theorem]]

The [[existence and uniqueness theorem]] for first-order ODEs states that for a given IVP:

$$y' = f(x,y), \quad y(x_0) = y_0$$

if $f(x,y)$ is continuous in a region containing $(x_0,y_0)$, then there exists a unique solution to the IVP in some interval around $x_0$. This theorem is crucial as it guarantees that a solution to an [[ODE]] exists and is unique under certain conditions.

## Separable Differential Equations

A separable differential equation is a type of first-order [[ODE]] where the dependent variable can be separated from the independent variable. It has the form:

$$\frac{dy}{dx} = g(x)f(y)$$

To solve this type of equation, we can use separation of variables by writing it as:

$$\frac{dy}{f(y)} = g(x)dx$$

and then integrating both sides with respect to their respective variables. For example, consider the following separable differential equation:

$$\frac{dy}{dx} = \frac{x}{y}$$

We can separate the variables as:

$$\frac{dy}{y} = xdx$$

and then integrate both sides to get:

$$\ln|y| = \frac{x^2}{2} + C$$

where $C$ is the constant of [[integration]]. Solving for $y$, we get:

$$y = Ce^{\frac{x^2}{2}}$$

## Homogeneous Differential Equations

A homogeneous differential equation is a type of first-order [[ODE]] where all terms can be expressed as a function of the ratio $\frac{y}{x}$. It has the form:

$$\frac{dy}{dx} = f\left(\frac{y}{x}\right)$$

To solve this type of equation, we can use the substitution $v = \frac{y}{x}$, which transforms the equation into a separable one. For example, consider the following homogeneous differential equation:

$$\frac{dy}{dx} = \frac{x-y}{x+y}$$

Using the substitution $v = \frac{y}{x}$, we get:

$$\frac{dv}{dx} + v = 0$$

This is now a separable differential equation, and we can solve it using separation of variables to get:

$$v = Ce^{-x}$$

Substituting back for $v$, we get the solution to our original equation as:

$$y = Cxe^{-x}$$

## Bernoulli Differential Equations

A Bernoulli differential equation is a type of first-order [[ODE]] with nonlinear terms in both the dependent variable and its [[derivative]]. It has the form:

$$\frac{dy}{dx} + p(x)y = q(x)y^n, \quad n \neq 1$$

To solve this type of equation, we can use the substitution $v = y^{1-n}$, which transforms it into a [[linear differential]] equation. For example, consider the following Bernoulli differential equation:

$$\frac{dy}{dx} + \frac{1}{x}y = y^2$$

Using the substitution $v = y^{-1}$, we get:

$$-\frac{dv}{dx} + \frac{1}{x}v = -1$$

This is now a [[linear differential]] equation, and we can solve it using an [[integrating factor]] to get:

$$v = Ce^{-\ln|x|} = Cx^{-1}$$

Substituting back for $v$, we get the solution to our original equation as:

$$y = \frac{1}{Cx + 1}$$

## Conclusion

In this atomic note, we discussed the basics of differential equations, including types of equations, notation, initial value problems, and key theorems. We also looked at three types of first-order ODEs: separable, homogeneous, and Bernoulli equations. These are just a few examples of the many techniques used to solve differential equations. With further study and practice, one can become proficient in solving more complex ODEs and PDEs.