#math #calc 
[[Integration]] by Parts is a technique used to evaluate integrals that arise when applying the [[Product Rule]] for differentiation. The formula is derived from the [[Product Rule]] and can be stated as follows:

If $u$ and $v$ are differentiable functions of $x$, then

$$\int u \, dv = uv - \int v \, du$$

This formula allows us to rewrite an [[integral]] in a way that may be easier to evaluate.

## Proof of [[Integration]] by Parts

To prove the [[integration]] by parts formula, we start with the [[Product Rule]] for differentiation:

$$\frac{d}{dx}(uv) = u \frac{dv}{dx} + v \frac{du}{dx}$$

Rearranging this equation, we can isolate one of the terms on one side:

$$u \frac{dv}{dx} = \frac{d}{dx}(uv) - v \frac{du}{dx}$$

Now, let's integrate both sides of this equation with respect to $x$:

$$\int u \, dv = \int \left(\frac{d}{dx}(uv) - v \frac{du}{dx}\right) dx$$

Applying the [[Fundamental Theorem of Calculus]] to the first term on the right-hand side:

$$\int u \, dv = uv - \int v \, du$$

This completes the proof of [[integration]] by parts.

## Example 1: Integrating a Product of Functions

Let's consider an example where we want to evaluate $\int x e^x dx$. We can use [[integration]] by parts in this case.

Choosing $u = x$ and $dv = e^x dx$, we have $du = dx$ and $v = e^x$. Applying the [[integration]] by parts formula:

$$\int x e^x dx = x e^x - \int e^x dx$$

Integrating the second term on the right-hand side gives:

$$\int x e^x dx = x e^x - e^x + C$$

where $C$ is the constant of [[integration]].

## Example 2: Repeated [[Integration]] by Parts

[[Integration]] by parts can be applied multiple times to evaluate more complicated integrals. Let's consider an example where we want to find $\int x^n \ln(x) dx$, where $n > 0$.

Choosing $u = \ln(x)$ and $dv = x^n dx$, we have $du = \frac{1}{x} dx$ and $v = \frac{x^{n+1}}{n+1}$. Applying [[integration]] by parts once:

$$\int x^n \ln(x) dx = \frac{x^{n+1}}{n+1} \ln(x) - \int \frac{x^{n+1}}{n+1} \cdot \frac{1}{x} dx$$

Simplifying the [[integral]] on the right-hand side, we get:

$$\int x^n \ln(x) dx = \frac{x^{n+1}}{n+1} \ln(x) - \frac{1}{(n+1)}\int x^n dx$$

The remaining [[integral]] can be evaluated straightforwardly as:

$$\int x^n \ln(x) dx = \frac{x^{n+1}}{n+1} \ln(x) - \frac{x^{n+1}}{(n+1)(n)} + C$$

where $C$ is the constant of [[integration]].

## Conclusion

[[Integration]] by Parts is a powerful technique for evaluating integrals that involve products of functions. By applying the formula derived from the [[Product Rule]] for differentiation, it allows us to rewrite integrals in a way that may be easier to solve. This technique can be particularly useful when dealing with logarithmic and exponential functions, as demonstrated in the examples above.