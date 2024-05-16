#diffeq #math 
The [[Laplace transform]] is a powerful mathematical tool used to solve differential equations. It transforms a function of time into a function of complex frequency, making it easier to analyze and solve problems in the frequency domain. One important property of the [[Laplace transform]] is its ability to handle derivatives.

## Definition

The [[Laplace transform]] of the [[Derivative]] of a function $f(t)$ is given by:

$$\mathcal{L}\{f'(t)\} = sF(s) - f(0)$$

where $F(s)$ is the [[Laplace transform]] of $f(t)$ and $s$ is the complex frequency variable.

## Proof

To prove this result, let's start with the definition of the [[Laplace transform]]:

$$F(s) = \mathcal{L}\{f(t)\} = \int_0^\infty e^{-st} f(t) dt$$

Now, let's differentiate both sides with respect to $s$:

$$\frac{d}{ds} F(s) = \frac{d}{ds} \int_0^\infty e^{-st} f(t) dt$$

Using [[Leibniz's rule]] for differentiating under the [[integral]] sign, we have:

$$\frac{d}{ds} F(s) = \int_0^\infty \frac{\partial}{\partial s}(e^{-st}) f(t) dt$$
$$\frac{d}{ds} F(s) = \int_0^\infty -te^{-st} f(t) dt$$

Now, let's rewrite this equation using [[Integration by Parts]]:

$$\frac{d}{ds} F(s) = [-te^{-st} f(t)]_0^\infty + \int_0^\infty e^{-st} f'(t) dt$$

Since we assume that $f(t)$ approaches zero as $t$ goes to infinity, the first term on the right-hand side becomes zero. Therefore, we have:

$$\frac{d}{ds} F(s) = \int_0^\infty e^{-st} f'(t) dt$$

Finally, taking the [[Laplace transform]] of both sides, we get:

$$sF(s) - f(0) = \mathcal{L}\{f'(t)\}$$

which is the desired result.

## Example

Let's apply this result to solve a simple [[Differential Equation]]. Consider the following initial value problem:

$$y''(t) + 2y'(t) + 2y(t) = 0, \quad y(0) = 1, \quad y'(0) = 0$$

Taking the [[Laplace transform]] of both sides using the [[Derivative]] property, we obtain:

$$s^2Y(s)-sy(0)-y'(0)+2(sY(s)-y(0))+2Y(s)=0$$

Substituting the initial conditions $y(0)=1$ and $y'(0)=0$, we simplify the equation to:

$$s^2Y(s)+2sY(s)+Y(s)-s-1=0$$

Rearranging terms and factoring out $Y(s)$, we have:

$$(s^2+2s+1)Y(s)=(s+1)$$

Simplifying further using the identity $(a+b)^2=a^2+2ab+b^2$, we get:

$$(s+1)^2 Y(s)=(s+1)$$

Dividing both sides by $(s+1)^2$, we obtain:

$$Y(s)=\frac{1}{(s+1)^2}$$

Now, let's find the [[inverse Laplace transform]] of $Y(s)$ to obtain the solution $y(t)$. Using the [[Laplace transform table]], we know that:

$$\mathcal{L}^{-1}\left\{\frac{1}{(s+a)^n}\right\} = t^{n-1} e^{-at}$$

Applying this result, we have:

$$y(t) = \mathcal{L}^{-1}\left\{\frac{1}{(s+1)^2}\right\} = t^{2-1} e^{-t}=te^{-t}$$

Therefore, the solution to the given [[Differential Equation]] is $y(t) = te^{-t}$.

This example demonstrates how the [[Laplace transform]] of derivatives can be used to solve differential equations more easily in the frequency domain.