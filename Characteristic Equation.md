#diffeq #math 
**Characteristic Equation in Differential Equations**

In [[linear]] homogeneous ordinary differential equations with constant coefficients, the characteristic equation is pivotal. For an $n$th [[order]] equation:

$a_n y^{(n)} + a_{n-1} y^{(n-1)} + \ldots + a_1 y' + a_0 y = 0$

Replace $y^{(k)}$ with $\lambda^k$, yielding a polynomial in $\lambda$, known as the characteristic equation. Solving this equation provides eigenvalues ($\lambda$) crucial for determining the general solution. 

**Example:**

Given $y'' - 3y' + 2y = 0$, replace derivatives: $\lambda^2 - 3\lambda + 2 = 0$. Factor to $(\lambda - 1)(\lambda - 2) = 0$, giving [[Eigenvalues]] $\lambda_1 = 1$ and $\lambda_2 = 2$. General solution: 

$y(t) = c_1 e^{\lambda_1 t} + c_2 e^{\lambda_2 t}$

1. **Distinct Real Roots ($r_1$ and $r_2$​)**: The general solution is $$y(x)=Ae^{r_1x}+Be^{r_2x}$$
2. **Repeated Real Roots ($r_1=r_2$​)**: The general solution is $$y(x) = (A+Bx)e^{rx}$$

3. **Complex Roots ($r_1=\alpha+i \beta$ and $r_2=\alpha- i \beta$)**: The general solution is $$y(x)=e^{\alpha x}(Acos(\beta x)+Bsin(\beta x))$$
