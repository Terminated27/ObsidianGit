#math #diffeq 
called [[homogeneous ODE]] if $g(t) \equiv 0$ otherwise non-homogenous

A second-[[order]] [[ordinary differential equation]] ([[ODE]]) is **[[homogeneous ODE]]** if all the terms in the equation involve the unknown function y and its derivatives, and there are no terms that are constants or functions of the independent variable x.

#### General form: 
$$a(t)\frac{d^2y}{dt^2}+b(t)\frac{dy}{dt}+c(t)y = 0$$
where a,b,c are constants

#### [[Characteristic Equation]]:

To solve the [[homogeneous second-order ODE]], we first find the **[[characteristic equation]]** by substituting $y=e^{rx}$ into the [[ODE]]. This yields:

$$ar^2+br+c=0$$

Solving this quadratic equation for r gives the characteristic roots. The solutions depend on the nature of the roots:

1. **Distinct Real Roots ($r_1$ and $r_2$​)**: The [[general solution]] is $$y(x)=Ae^{r_1x}+Be^{r_2x}$$
2. **Repeated Real Roots ($r_1=r_2$​)**: The [[general solution]] is $$y(x) = (A+Bx)e^{rx}$$

3. **Complex Roots ($r_1=\alpha+i \beta$ and $r_2=\alpha- i \beta$)**: The [[general solution]] is $$y(x)=e^{\alpha x}(Acos(\beta x)+Bsin(\beta x))$$


Where $A$ and $B$ are constants determined by [[initial condition]]s if given.

#### Example:
let's solve the [[ODE]] 
$$
\begin{cases}
y''-3y'+2y=0\\
y(0)=1\\
y'(0)=2
\end{cases} 
$$
1. **[[Characteristic Equation]]**
	- $r^2-3r+2y=0$
	- solving for [[Root]]s we get $r_1=1$ and $r_2=2$
2. **[[General Solution]]**
	- $y(x)=Ae^{r_1x}+Be^{r_2x}$
3. **Apply [[initial condition]]s**
	- $$\begin{cases}
y(0)=A+B = 1\\
y'(0)=A(1)+2B(2)=2
\end{cases}$$
	- A = -1 , B = 2
4. **Particular Solution**
	- $y(x)=-e^{x}+2e^{2t}$


  