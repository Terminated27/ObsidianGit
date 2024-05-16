#math #diffeq 
Written in the form: $$a(t)\frac{d^2y}{dt^2}+b(t)\frac{dy}{dt}+c(t)y = f(t)$$
To solve this equation, typically follow:
1. **Find [[General Solution]]**
	-  First, find the solutions of the corresponding [[homogeneous ODE|homogenous]] equation $$a(t)\frac{d^2y}{dt^2}+b(t)\frac{dy}{dt}+c(t)y = 0$$
	- Depending on the [[Root]]s of the [[Characteristic Equation]], the [[General Solution]] can be of 3 types [[Overdamped]], [[Underdamped]], or [[Critically Damped]]
2. **Find a Particular Solution**
	-  Find a particular solution for the given non-homogenous term $f(t)$. The method for finding this solution depends on the form of $f(t)$ . Common methods include undetermined coefficients, variation of parameters, and [[Laplace Transform]]
3. **Combine the solutions**
	- Combine the [[general solution]] of the homogeneous equation and the particular solution to get the [[general solution]] of the non-homogeneous equation.
1. **Apply Initial Conditions or Boundary Values (if any):**
    - If you have initial conditions or boundary values, use them to determine the constants in the [[general solution]].
2. **Simplify and Interpret the Result:**
    - Simplify the solution if necessary and interpret the result in the context of the problem you are solving.
[[Existence and Uniqueness Theorem]]
