#math #diffeq 
Def.
a first order [[ODE]] is called separable if it has the form of $$M(x)+N(y)\frac{dy}{dx}=0$$
where M and N are given one variable functions
Def
consider [[ODE]] $\frac{dy}{dx}=f(x,y)$
if $f(tx,ty)=f(x,y)$ for any nonzero real number t
then the [[ODE]] is said to be [[homogeneous ODE|homogenous]]


once we found that an [[ODE]] is separable then observe that by [[integral|integrating]] both sides $$\int_{x_0}^x M(s)ds+\int_{y_0}^y N(y(s)\frac{dy}{ds}ds$$
or, if we are not given the [[initial condition]]
$$\int M(x)dx+\int N(y) dy = C$$
c is arbitrary constant

# Examples
## Example 1
show that the [[ODE]] $$\frac{dy}{dx}=\frac{x^2}{1-y^2}$$
is separable and find the solution
### solution 
1. by multiplying $(1-y^2)$ on both sides $(1-y^2)\frac{dy}{dx}=x^2$
$x^2+(y^2-1)\frac{dy}{dx}=0$
2. the [[ODE]] is separable w/ $M(x)=x^2$, $N(y)=y^2-1$
now observe that 
$\int M(x)dx+\int N(y) dy$
3. plug in and integrate
$\frac13x^3+\frac13y^3-y=C$
then any y/x satisfying the equation above is a solution

## Example 2
solve the initial value problem
$$\frac{dy}{dx}=\frac{3x^2+4x+2}{2(y-1)}$$
$$y(0)=-1$$
and determine the interval in which the solution exists
### Solution
1. put all variables on one side
$(3x^2+4x+2)+2(y-1)\frac{dy}{dx}$
2. then this [[ODE]] is separable with 
$M(x)=3x^2+4x+2$
$N(y)=2(y-1)$
3. since we have an [[initial condition]]
$y(0)=-1$
$\int_0^x(3x^2+4x+2)dx+\int_{-1}^y2(1-y)dy=0$
get the 0 from the 0 in y(0) and -1 from y(0)=-1
4. simplify down to get
$x^3+2x^2+2x+2y-y^2+3=0$
therefore
$y^2-2y-(x^3+2x^2+2x+3)$
by using [[quadratic formula]] $$\frac{-b\pm \sqrt{b^2-4ac}}{2a}$$
$\frac{2\pm \sqrt{2^2+4(x^3+2x^2+2x+3)}}{2}$
$1\pm \sqrt{x^3+2x^2+2x+4}$
5. let us check the [[initial condition]]
$(x=0$, $y=-1)$
$-1 = 1\pm \sqrt{0+0+0+4}$
only minus version is correct because it needs to be negative
$y=1- \sqrt{x^3+2x^2+2x+4}$
6. now we investigate the [[interval of validity]]
observe that $x^3+2x^2+2x+4\ge0$

let $f(x)=x^3+2x^2+2x+4$
note that 
$f(-2)=-8+8-4+4 = 0$
$f(x)=(x+2)(x^2+2)$
as long as $(x+2)\ge0$, $f(x)\ge0$ so we are good
thus the interval is $x\ge-2$, $[-2, \infty)$
on this interval, the [[initial condition]] is true
## Example 3
Solve the [[ODE]]
$$\frac{dy}{dx}=\frac{4x-x^3}{4+y^3}$$
and find the solution passing (0,1) and determine its [[interval of validity]]
### Solution
1. get all var on one side
$(x^3-4x)+(y^3+4)\frac{dy}{dx}=0$
2. it is separable w/
$M(x)=x^3-4x$
$N(y)=y^3+4$
3. $\int M(x)dx+\int N(y) dy$
$\frac14x^4-2x^2+\frac14y^4+4y=C$
for arbitrary constant C
now lets find the particular solution passing (0,1)
$x=0, y=1$
$0-0+1+16=C$
$C=17$
so our particular solution is $x^4-8x^2+y^4+16y=17$
## Example 4
Find the [[General Solution]] to the following [[ODE]]
$$\frac{dy}{dx}=\frac{y-4x}{x-y}$$
[[non-linear]], not separable

### Solution
let $f(x,y) = \frac{y-4x}{x-y}$
observe that
$f(tx,ty)=\frac{ty-4tx}{tx-ty}$
cancel out
$f(tx,ty)=\frac{t(y-4x)}{t(x-y)}$
$f(tx,ty)=\frac{y-4x}{x-y}$
$f(tx,ty)=f(x,y)$

Thus the [[ODE]] is [[homogeneous ODE|homogenous]]
because it is not separable
define a variable $v=\frac yx;vx=y$ to force it to be separable
$\frac{dy}{dx}=\frac{d}{dx}(vx)=v+xv'$
$f(x,y)=\frac{vx-4x}{x-vx}=\frac{v-4}{1-v}$
thus $\frac{dy}{dx}=f(x,y)$
$v'=\frac1x(\frac{v-4}{1-v}-v)$
$v'=\frac1x(\frac{v^2-4}{1-v})$
$\frac{dv}{dx}$
