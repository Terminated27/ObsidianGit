#math #diffeq 

decide if [[separable ODE]] and [[Linear Differential]]
shortcuts

example using the [[differential equation]] $\frac{dy}{dx}=10-\frac{y}{5}$​ with an initial condition y(0)=20. Here are the steps:

**Step 1: Rewrite the [[ODE]]**

- Write the [[ODE]] in [[standard form]], isolating $\frac{dy}{dx}$​ on one side: $\frac{dy}{dx}+\frac15y=10$.

**Step 2: Recognize the Linear First-Order [[ODE]]**

- Notice that this is a linear first-order [[ordinary differential equation]]. It has the form $\frac{dy}{dx}+P(x)y=Q$, where $P(x)=\frac15$​ and $Q(x)=10$.

**Step 3: Solve Using an [[Integrating Factor]]**

- To solve this linear [[ODE]], you can use an [[integrating factor]], denoted as μ(x), which is given by: $\mu(x)=e^{\int P(x)dx}$.  
- In our case, $\mu(x)=e^{\int \frac 15dx}=e^\frac x5$.

**Step 4: Multiply Both Sides by the [[Integrating Factor]]**

- Multiply the entire [[ODE]] by the [[integrating factor]] μ(x): $e^\frac x5\frac{dy}{dx}+\frac15e^{\frac x5}y=10e^{\frac{x}{5}}$.

**Step 5: Apply the [[Product Rule]] on the Left Side**

- Recognize that the left side is now the [[Derivative]] of the product of μ(x) and y. Apply the [[product rule]]: $e^\frac x5\frac{dy}{dx}+\frac15e^{\frac x5}y=10e^{\frac{x}{5}}$.
- The [[product rule]] gives: $\frac{d}{dx}(e^{\frac x5}y)=10e^{\frac x5}$.
    

**Step 6: Integrate Both Sides**

- [[Integral|Integrate]] both sides with respect to x.
	$\int \frac{d}{dx}(e^{\frac x5}y)dx=\int10e^{\frac{x}{5}}dx$

- On the left side, the [[integral]] of a [[derivative]] is simply the original function:
	$e^{\frac x5}y=50e^{\frac x5}+C$, 
	where C is the constant of [[integration]].
    

**Step 7: Solve for y**

- Isolate y by dividing both sides by $e^{\frac x5}$: $y=50+Ce^{-\frac x5}$.

**Step 8: Incorporate the Initial Condition**

- Use the initial condition y(0)=20 to solve for the constant C: $10=50+Ce^0$.
    
- Simplify: C=20−50=−30.
    

**Step 9: Final Solution**

- Substitute the value of C back into the equation: $y=50-30e^{-\frac x5}$.

That's the solution for y that satisfies the given initial condition and the [[differential equation]].