#math #diffeq 

**Reduction Method in Differential Equations**

The reduction method is a technique used to solve first-[[order]] [[linear]] ordinary differential equations. These equations are of the form:

$$\frac{dy}{dx} + P(x)y = Q(x)$$

where $P(x)$ and $Q(x)$ are functions of $x$. To solve this equation, the [[integrating factor]] $I(x)$ is introduced, defined as:

$$I(x) = e^{\int P(x)dx}$$

Multiplying both sides of the original equation by $I(x)$ results in:

$$e^{\int P(x)dx} \frac{dy}{dx} + e^{\int P(x)dx}P(x)y = e^{\int P(x)dx}Q(x)$$

The left side can be rewritten using the [[Product Rule]], allowing [[integration]] of both sides to find $y(x)$.

**Example:**

Consider the equation:

$$\frac{dy}{dx} + 2xy = x$$

First, identify $P(x) = 2x$ and $Q(x) = x$. The [[integrating factor]] is:

$$I(x) = e^{\int 2xdx} = e^{x^2}$$

Multiplying the given equation by the [[integrating factor]]:

$$e^{x^2} \frac{dy}{dx} + 2xe^{x^2}y = xe^{x^2}$$

Now, notice that the left side is the result of the [[Product Rule]] applied to $(e^{x^2}y)$. Integrating both sides:

$$e^{x^2}y = \int xe^{x^2}dx$$

Solving the [[integral]] on the right side and simplifying gives $y(x)$.