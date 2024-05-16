#math #diffeq 

**Nonhomogeneous Second [[Order]] [[ODE]] with Constant Coefficients**

A nonhomogeneous second-[[order]] ordinary [[Differential Equation]] ([[ODE]]) with constant coefficients has the form:

$$a y''(x) + b y'(x) + c y(x) = F(x)$$

where $a$, $b$, and $c$ are constants, and $F(x)$ represents a nonhomogeneous function of $x$. To solve this equation, a particular solution $y_p(x)$ for the nonhomogeneous part is found. The [[general solution]] is then the sum of the particular solution and the complementary function $y_c(x)$, which solves the associated homogeneous equation:

$$a y''(x) + b y'(x) + c y(x) = 0$$

The complementary function $y_c(x)$ is found by assuming $y(x) = e^{rx}$ and solving the [[characteristic equation]]:

$$ar^2 + br + c = 0$$

Once the roots $r_1$ and $r_2$ of the [[characteristic equation]] are found, the complementary function is given by:

$$y_c(x) = C_1 e^{r_1x} + C_2 e^{r_2x}$$

where $C_1$ and $C_2$ are constants determined by initial or boundary conditions.

To find the particular solution $y_p(x)$, various methods like undetermined coefficients, variation of parameters, or [[integrating factor]]s can be employed, depending on the form of $F(x)$. Once $y_p(x)$ is determined, the [[general solution]] of the nonhomogeneous equation is:

$$y(x) = y_c(x) + y_p(x)$$

Solving nonhomogeneous second-[[order]] [[ODE]]s with constant coefficients often involves a combination of algebraic manipulation and understanding the properties of the nonhomogeneous term $F(x)$.

### example
Let's consider a specific example of a nonhomogeneous second-[[order]] [[ordinary differential equation]] with constant coefficients:

$$y''(x) - 3y'(x) + 2y(x) = 2e^x$$

**Solution:**

First, solve the associated homogeneous equation:

$$y''(x) - 3y'(x) + 2y(x) = 0$$

The [[characteristic equation]] is:

$$\lambda^2 - 3\lambda + 2 = 0$$

Factoring the [[characteristic equation]] gives $(\lambda - 1)(\lambda - 2) = 0$, which yields $\lambda_1 = 1$ and $\lambda_2 = 2$.

So, the complementary function is:

$$y_c(x) = C_1 e^{x} + C_2 e^{2x}$$

Next, for the particular solution, [[guess a form for y_p(x)]] based on the nonhomogeneous term $2e^x$. Since $e^x$ is part of the complementary function, a suitable guess is: (because an equivalent to $Ae^x$ already is in the [[Characteristic Equation]], you need to multiply by $x^2$ or $x$ to make it not cancel out)

$$y_p(x) = Ax^2e^x$$

Now, find the first and second derivatives of $y_p(x)$:

$$y'_p(x) = (2Ax + Ax^2)e^x$$
$$y''_p(x) = (2A + 2Ax + 2Ax^2)e^x$$

Substitute these derivatives and $y_p(x)$ into the original nonhomogeneous equation:

$$(2A + 2Ax + 2Ax^2 - 3(2Ax + Ax^2) + 2(Ax^2e^x))e^x = 2e^x$$

Simplify and [[Equating Coefficients in Differential Equations]] to find the value of $A$.
 
Once $A$ is determined, the particular solution is found. The [[general solution]] for the nonhomogeneous equation is the sum of the complementary function and the particular solution:

$$y(x) = y_c(x) + y_p(x) = (C_1 e^{x} + C_2 e^{2x}) + (Ax^2e^x)$$

Here, $C_1$, $C_2$, and $A$ are constants determined by initial conditions if provided.