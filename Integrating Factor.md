#math #diffeq #calc 

The integrating factor is a mathematical tool used to solve linear ordinary differential equations (ODEs) of the form:

$$\frac{{dy}}{{dx}} + P(x)y = Q(x)$$

where $P(x)$ and $Q(x)$ are continuous functions of $x$. The integrating factor allows us to transform this equation into a more easily solvable form.

## Definition

Given an [[ODE]] of the form $\frac{{dy}}{{dx}} + P(x)y = Q(x)$, the integrating factor $I(x)$ is defined as:

$$I(x) = e^{\int P(x) \, dx}$$

## Theorem 1: Multiplying by the Integrating Factor

If we multiply both sides of the [[ODE]] $\frac{{dy}}{{dx}} + P(x)y = Q(x)$ by the integrating factor $I(x)$, we obtain:

$$I(x)\frac{{dy}}{{dx}} + I(x)P(x)y = I(x)Q(x)$$

The left-hand side can be rewritten as:

$$\frac{{d}}{{dx}}(I(x)y) = I'(x)y + I(x)\frac{{dy}}{{dx}}$$

Therefore, our equation becomes:

$$\frac{{d}}{{dx}}(I(x)y) = I'(x)y + I(x)\frac{{dy}}{{dx}} = I(x)Q(X)$$

## Theorem 2: Solving the [[ODE]] with Integrating Factor

By applying Theorem 1, we have transformed our original [[ODE]] into the following equation:

$$\frac{{d}}{{dx}}(I(X)y) = I(X)Q(X)$$

Integrating both sides with respect to $x$, we get:

$$I(X)y = \int I(X)Q(X) \, dx + C$$

where $C$ is the constant of [[integration]]. Finally, we can solve for $y$:

$$y = \frac{{\int I(X)Q(X) \, dx + C}}{{I(X)}}$$

## Example

Let's consider the following [[ODE]]:

$$\frac{{dy}}{{dx}} + 2xy = x^2$$

To solve this using the integrating factor, we first identify $P(x) = 2x$ and $Q(x) = x^2$. The integrating factor is then given by:

$$I(x) = e^{\int 2x \, dx} = e^{x^2}$$

Multiplying both sides of the [[ODE]] by the integrating factor, we have:

$$e^{x^2}\frac{{dy}}{{dx}} + 2xe^{x^2}y = x^2e^{x^2}$$

Applying Theorem 1, we rewrite this equation as:

$$\frac{{d}}{{dx}}(e^{x^2}y) = x^2e^{x^2}$$

Integrating both sides with respect to $x$, we get:

$$e^{x^2}y = \int x^2e^{x^2} \, dx + C$$

Simplifying the [[integral]] on the right-hand side, we have:

$$e^{x^2}y = \frac{1}{3}x^3e^{x^3} + C$$

Finally, solving for $y$, we obtain:

$$y = \frac{1}{3}x^3 + Ce^{-x^3}, \quad C \in \mathbb{R}$$