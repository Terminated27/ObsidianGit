#math #diffeq 
Steps for solve



for [[Exact Differential Equation]]
can be applied to [[separable ODE]] and [[First Order ODE]]
for an equation that can be split up into M(x,y) and N(x,y)
written as M(x, y) dx + N(x, y) dy = 0
if ($\frac{\partial}{\partial y}$ of M) = ($\frac{\partial}{\partial x}$ of N) ([[Partial Derivative]]) then the equation is exact. 
then you can set $\Psi$ equal to M and N
$$\Psi_x(x,y)=m(x,y)$$
$$\Psi_y(x,y)=n(x,y)$$
then integrate both sides of one equation
$$\int \Psi_x dx= \int mdx$$
the resultant constant can be called h(y) <-- y in this situation because it is respect to x, h(y) should not depend on x, ie. there is no x in h, or h'
$$\Psi_y(x,y)=(n(x,y))+h'(y)$$
because h(y) is a constant, h'(x) = 0
therefore, $\Psi(x,y) = (\int m dx)+C$
C = solution
then to solve for h(y), plug [[derivative]] into n (or m depending)
 solve for h using h'

https://www.youtube.com/watch?v=bwASJWS8ltM

# [[separable ODE]]
$M_y(x,y) = \frac{\partial}{\partial y}m(x) = 0$
$N_x(x,y) = \frac{\partial}{\partial x}n(y) = 0$
[[separable ODE]] is always exact
# [[First Order ODE]]
$p(x)y+\frac{d}{dy}=q(x)$
$p(x)y-q(x)+\frac{d}{dy}=0$
use [[Integrating Factor]] ($e^{\int p(x) dx}$) to move around to get 
$e^{\int p(x) dx}(p(x)y-q(x)+e^{\int p(x) dx}y'=0$
let $M(x,y) = e^{\int p(x) dx}(p(x)y-q(x)$
$N(x,y) = e^{\int p(x) dx}$
[[partial derivative]] of both is equal $\therefore$ exact