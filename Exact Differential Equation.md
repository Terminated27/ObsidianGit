#math #diffeq 

An exact [[Differential Equation]] is a type of first-[[order]] [[ordinary differential equation]] ([[ODE]]) that can be written in the form:

$$M(x,y)dx + N(x,y)dy = 0$$

where $M$ and $N$ are functions of two variables $x$ and $y$. 

## Definition

A first-[[order]] [[ODE]] is said to be exact if [[there exists]] a function $\phi(x,y)$ such that:

$$\frac{\partial \phi}{\partial x} = M(x,y) \quad \text{and} \quad \frac{\partial \phi}{\partial y} = N(x,y)$$

In other words, the partial derivatives of $\phi$ with respect to $x$ and $y$ are equal to $M(x,y)$ and $N(x,y)$, respectively.

## Theorem 1: Test for Exactness

A necessary condition for a first-[[order]] [[ODE]] to be exact is that:

$$\frac{\partial M}{\partial y} = \frac{\partial N}{\partial x}$$

If this condition is satisfied, then the [[ODE]] may be exact. However, it does not guarantee exactness.

## Theorem 2: [[Integrating Factor]]

If a first-[[order]] [[ODE]] is not exact, but satisfies the condition $\frac{\partial M}{\partial y} - \frac{\partial N}{\partial x} = P(x,y)$ (where $P(x,y)$ is a function), then an [[integrating factor]] $\mu(x,y)$ can be found such that:

$$\mu(x,y) \left(M(x,y)dx + N(x,y)dy\right)$$

is an exact differential.

The [[integrating factor]] $\mu$ is given by:

$$\mu = e^{\int P(x,y) dx}$$

## Proof of Theorem 2

To prove Theorem 2, let's consider the equation:

$$\frac{\partial \mu M}{\partial y} = \frac{\partial \mu N}{\partial x}$$

Expanding the partial derivatives and simplifying, we get:

$$M \frac{\partial \mu}{\partial y} + \mu \frac{\partial M}{\partial y} = N \frac{\partial \mu}{\partial x} + \mu \frac{\partial N}{\partial x}$$

Rearranging the terms, we have:

$$M \frac{\partial \mu}{\partial y} - N \frac{\partial \mu}{\partial x} = -\left(\frac{\partial M}{\partial y} - \frac{\partial N}{\partial x}\right) \mu$$

Comparing this with the condition $\frac{\partial M}{\partial y} - \frac{\partial N}{\partial x} = P(x,y)$, we can see that:

$$M \frac{\partial \mu}{\partial y} - N \frac{\partial \mu}{\partial x} = -P(x,y) \mu$$

This is a first-[[order]] [[linear]] partial [[Differential Equation]] for $\mu$. Solving this equation gives us the [[integrating factor]] $\mu$.
## Example

Let's consider the following [[ODE]]:

$$(3x^2y^2 + 2xy)dx + (x^3y + 3xy^2)dy = 0$$

We can check if it is exact by computing the partial derivatives:

$$M(x,y) = 3x^2y^2 + 2xy,\\
N(x,y) = x^3y + 3xy^2,$$

and then verifying if $\frac{{\rm d}}{{\rm d}y}M(x,y) = \frac{{\rm d}}{{\rm d}x}N(x,y)$:

$$\frac{{\rm d}}{{\rm d}y}(3x^2y^2 + 2xy) = 6xy^2 + 2x,\\
\frac{{\rm d}}{{\rm d}x}(x^3y + 3xy^2) = 3x^2y + 6xy.$$

Since the condition is not satisfied, we can proceed to find the [[integrating factor]] $\mu$:

$$P(x,y) = \frac{{\rm d}}{{\rm d}y}(3x^2y^2 + 2xy) - \frac{{\rm d}}{{\rm d}x}(x^3y + 3xy^2) = -4xy.$$

Using the formula for the [[integrating factor]], we have:

$$\mu = e^{\int P(x,y) dx} = e^{-2xy},$$

Multiplying the original [[ODE]] by the [[integrating factor]] $\mu = e^{-2xy}$, we have:

$$e^{-2xy}[(3x^2y^2 + 2xy)dx + (x^3y + 3xy^2)dy] = 0.$$

Expanding and simplifying, we get:

$$(3x^2y^2e^{-2xy} + 2xye^{-2xy})dx + (x^3ye^{-2xy} + 3xy^2e^{-2xy})dy = 0.$$

Now, let's define a new function $F(x,y)$ such that:

$$\frac{{\partial F}}{{\partial x}} = 3x^2y^2e^{-2xy} + 2xye^{-2xy},\\
\frac{{\partial F}}{{\partial y}} = x^3ye^{-2xy} + 3xy^2e^{-2xy}.$$

To find $F(x,y)$, we integrate the first equation with respect to $x$:

$$F(x,y) = \int (3x^2y^2e^{-2xy} + 2xye^{-2xy})dx.$$

Integrating term by term, we have:

$$F(x,y) = \int 3x^4y^4 e^{-2xy} dx + \int  6x^3y e^{-2xy} dx.$$

For the first [[integral]], we can use [[integration by parts]] with $u = x$ and $dv = x^3y^{4} e^{-{4yx}} dx$. This gives us $du=dx$ and $v=-\frac{1}{4}\left( y^{4}\right)e^{ -4yx}$. Applying the [[integration by parts]] formula, we have:

$$\int 3x^4y^4 e^{-2xy} dx = -\frac{3}{4} x^{3} y^{4} e^{-2xy}- \int -\frac{1}{4}\left( y^{4}\right)e^{ -4yx} dx.$$

Simplifying further, we have:

$$F(x,y) = -\frac{3}{4} x^{3} y^{4} e^{-2xy}- \int -\frac{1}{4}\left( y^{4}\right)e^{ -4yx} dx + 6x^3y e^{-2xy}.$$

Now, let's integrate the second [[integral]] $\int -\frac{1}{4}\left( y^{4}\right)e^{ -4yx} dx$. We can use substitution with $u = -2yx$ and $du = -2ydx$. This gives us:

$$-\int \frac{1}{8}\left( y^{3}\right)e^{ u } du =-\frac{1}{8}\left( y^{3}\right)e^u.$$

Substituting back $u$ and simplifying, we have:

$$-\int \frac{1}{8}\left( y^{3}\right)e^{-2yx } dx =-\frac{1}{8}\left( y^{3}\right)e^{-2xy }.$$

Now, substituting this result back into our expression for $F(x,y)$, we have:

$$F(x,y) = -\frac{3}{4} x^{3} y^{4} e^{-2xy}- \left(-\frac{1}{8}\left( y^{3}\right)e^{-2xy }\right) + 6x^3y e^{-2xy}.$$

Simplifying further, we get:

$$F(x,y) = -\frac{3}{4} x^{3} y^{4} e^{-2xy} +\frac{1}{8}\left( y^{3}\right)e^{-2xy } + 6x^3y e^{-2xy}.$$

Finally, the solution to the exact [[Differential Equation]] is given by $F(x,y) = C$, where $C$ is a constant.