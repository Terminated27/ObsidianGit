#math #diffeq 

- [[Linearize|Linearizing]] an [[ODE]] involves simplifying a [[nonlinear differential equation]] into a linear form around a specific operating point or equilibrium.
- The [[linearize|linearlization]] is typically achieved by using [[Taylor series]] or [[small perturbation methods]] to approximate nonlinear terms with linear terms.
- Once [[linearize|linearized]], the [[ODE]] can often be solved more easily using linear algebraic techniques or well-established methods for solving [[linear differential equations]].

# example

Suppose we have the following nonlinear [[ODE]]:

$$\frac{dy}{dx} = y^2 -1$$

We want to linearize this [[ODE]] around an [[equilibrium point]], let's say $y=1$

**Step 1: Find the [[Equilibrium Point]]** To linearize the [[ODE]], we first need to find the equilibrium point, where the right-hand side $y^2-1$ equals zero:

$y^2-1=0$

Solving for y, we get $y=\pm 1$. So, our equilibrium point is y=1.

**Step 2: Linearize the [[ODE]]** To linearize the [[ODE]], we'll introduce a small deviation from the equilibrium point:

$$y=1+\delta$$

Where δ represents a small change in y around the equilibrium point.

**Step 3: Express the [[ODE]] with the Small Deviation** Now, substitute y=1+δ into the original [[ODE]]:

$$\frac{d(1+\delta)}{dt}=(1+\delta)^2-1$$

**Step 4: Simplify and Approximate** Expand and simplify the equation:

$$\frac{d \delta}{dt}=\delta^2+2\delta$$

Now, we'll make an approximation. If δ is small, then $δ^2$ is much smaller. So, we can approximate $δ^2$ as approximately zero:

$$\frac{d \delta}{dt}\approx2\delta$$

**Step 5: Solve the Linearized [[ODE]]** The linearized [[ODE]] is a first-order linear [[ODE]]:

$$\frac{d \delta}{dt}=2\delta$$

This is a simple linear [[ODE]] with a known solution. The solution is:

$$\delta(t)=\delta_0e^{2t}$$
Where $\delta_0$ is the initial deviation from the equilibrium point at t=0.

**Step 6: Incorporate the Solution Back** Now that we have the solution for δ(t), we can incorporate it back to find the solution for y(t):

$$y(t)=1+\delta(t) = 1+\delta_0e^{2t}$$

So, the solution to the original nonlinear [[ODE]] is given by:

$$y(t)=1+\delta0e^{2t}$$

This is the approximate solution to the nonlinear [[ODE]] near the equilibrium point y=1 using linearization.