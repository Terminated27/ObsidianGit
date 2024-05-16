#calc #math 
## Definition
The double [[integral]] is an extension of the concept of a single [[integral]] to functions of two variables over a region in the plane. It represents the volume under the surface defined by the function.

For a function $f(x,y)$ defined over a region $R$ in the $xy$-plane, the double [[integral]] is denoted as:

$$\iint_R f(x,y) \, dA$$

where $dA$ represents an infinitesimal area element.

## Iterated Integrals
To evaluate a double [[integral]], we can use iterated integrals. There are two types: Type I and Type II.

### Type I Iterated [[Integral]]
For a region $R$ defined by $a \leq x \leq b$, $c \leq y \leq d$, where $a < b$ and $c < d$, the Type I iterated [[integral]] is given by:

$$\iint_R f(x,y) \, dA = \int_a^b\int_c^d f(x,y) \, dydx$$

### Type II Iterated [[Integral]]
For a region $R$ defined by $\alpha \leq y \leq \beta$, $\gamma(y) \leq x \leq \delta(y)$, where $\alpha < \beta$ and $\gamma(y) < \delta(y)$ for all $y$ in the interval $(\alpha,\beta)$, the Type II iterated [[integral]] is given by:

$$\iint_R f(x,y) \, dA = \int_\alpha^\beta\int_{\gamma(y)}^{\delta(y)} f(x,y) \, dxdy$$

## Properties of Double Integrals
1. Linearity: $$\iint_R (af(x,y) + bg(x,y))  dA = a\iint_R f(x,y) dA + b\iint_R g(x,y) dA$$
2. Reversing the Order: $$\iint_R f(x,y) dA = \iint_S f(x,y) dA$$

## Fubini's Theorem
Fubini's theorem states that if $f(x,y)$ is integrable over a rectangle $R$, then the double [[integral]] of $f$ over $R$ can be computed by either of the following iterated integrals:

$$\iint_R f(x,y) \, dA = \int_a^b\int_c^d f(x,y) \, dydx = \int_c^d\int_a^b f(x,y) \, dxdy$$
## Example
Evaluate the double [[integral]] $\iint_R (6x + 2y) \, dA$, where $R$ is the region defined by $0 \leq x \leq 1$ and $0 \leq y \leq 2$.

Using Type I iterated [[integral]]:

$$\begin{align*}
\iint_R (6x + 2y) \, dA &= \int_0^1\int_0^2 (6x + 2y) \, dydx \\
&= \int_0^1 [6xy + y^2]_0^2 dx \\
&= \int_0^1 (12x + 4) dx \\
&= [6x^2 + 4x]_0^1 \\
&= (6(1)^2 + 4(1)) - (6(0)^2 + 4(0)) \\
&= 10
\end{align*}$$

Therefore, $\iint_R (6x + 2y) \, dA = 10$.

Note: The order of [[integration]] could be reversed by using the Type II iterated [[integral]] as well.