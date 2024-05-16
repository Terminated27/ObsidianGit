#math #diffeq 
#### **Definition:** 
The Wronskian, denoted as
$W(f,g)(x)$ or $W[f,g](x)$ is a mathematical [[determinant]] used to determine the [[linear independence]] of 2 functions f(x) and g(x) or to find solutions to [[linear differential equations]] 
#### For 2 Functions
f(x) and g(x) defined on an interval $I$ , the [[Wronskian]] is given by formula:
$$
W(f,g)(x) =
\begin{vmatrix}
f(x)&g(x)\\
f'(x)&g'(x)
\end{vmatrix}
=f(x)g'(x)-f'(x)g(x)
$$
#### Linear Independence
if $W(f,g)(x)\ne0$ for all x in the interval $I$, then f(x) and g(x) are [[linearly independent]] on $I$
#### Application in [[Differential Equation]]s
Given a [[Homogeneous second-order ODE]] $y''(x)+p(x)y'(x)+q(x)y(x)=0$ two solutions $y_1(x)$ and $y_2(x)$ are [[linearly independent]] $\iff$ $W(y_1,y_2)(x_0)\ne 0$ for some point $x_0$ in the interval $I$
##### Solving [[Differential Equation]]s
The Wronskian can be used to find a second linearly independent solution of a [[differential equation]] if one solution is known. If $y_1(x)$ is a known solution, another linearly independent solution can be found using the formula:
#### Properties
- if $W(f,g)(x)=0$ for all in x in an interval $I$, then f(x) and g(x) are [[linearly dependent]] on $I$
- The [[Wronskian]] satisfies the [[Wronskian]] [[Differential Equation]]: $W'(x)=p(x)W(x)$, where p(x) is a given function
#### **Solving Differential Equations:**
The Wronskian can be used to find a second linearly independent solution of a [[differential equation]] if one solution is known. If $y_1(x)$ is a known solution, another linearly independent solution can be found using the formula:
$$y_2(x)=y_1(x)\int \frac{1}{y_1^2(x)}e^{-\int p(x)dx}dx$$
#### Non-homogeneous equations:
**Solving Differential Equations:** The Wronskian can be used to find a second linearly independent solution of a [[differential equation]] if one solution is known. If $y_1​(x)$ is a known solution, another linearly independent solution can be found using the formula:
IDK LOL
#### Higher Order [[Differential Equation]]s
The concept of the Wronskian can be extended to higher order differential equations. For a [[set]] of $n$ functions $y_1​(x),y_2​(x),\dots,y_n​(x)$, the Wronskian determinant is defined as:
$$
W(y_1,y_2,...,y_n)(x)=
\begin{vmatrix}
y_1(x)&y_2(x)&\dots& y_n(x)\\
y'_1(x)&y'_2(x)&\dots& y'_n(x)\\
\vdots&\vdots&\ddots&\vdots\\
y^{n-1}_1(x)&y^{n-1}_2(x)&\dots& y^{n-1}_n(x)
\end{vmatrix}
$$
where $y^k(x)$ represents the kth [[derivative]] of y(x)