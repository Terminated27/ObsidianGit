#math #diffeq 
1. we need to know how to model [[First Order ODE]]
	1. figure out all the variables relevant to the situation
	2. figure out all the rules governing the situation
	3. choose unit
	4. combine all and get [[ODE]]
2. analyze the model
	1. find the solution
	2. in case it is [[non-linear]] and not [[separable ODE|separable]], [[Linearize]] it
3. comparison with experiment and observation
	1. we need to check if the solution of the [[ODE]] behaves physically reasonable
	2. calculate the solution for same parameters and compare with our experiment or observation
	3. check if the long time behavior is constant with out observation


# Examples
## ex1
![[Pasted image 20230919101553.png]]
want to investigate a(t): the amount of salt in the tank
$\frac{dq}{dt} = \frac{r}4-\frac{Qr}{100}$
same as first homework
[[separable ODE]]
$=\frac{r}{100}(25-Q)$
in photos, one with his arm and the right side of the board
simplify to $Q=25+Ce^{\frac{-rt}{100}}$
as t approach $\infty$ the e part goes to 0 and Q=25

### part 2

if $r=3$ $Q_0=2Q_L$ find the time T after which the salt level is within 2% of $Q_L$
 $$Q(t)=25+(Q_0-2T)e^{-\frac{rt}{100}}$$
 in photos

## ex2

MEMORIZEABLE SOLUTION

compounding interest
initial money = $S_0$
after 1 year = $S+rS$
we want to investigate the amount of money S(t)
find the difference between initial and after 1 year
$$\frac{dS}{dt}=rS$$
assuming the return is continuous

$\frac{dS}{dt}=rS$
$S(0)=S_0$
[[separable ODE]]


## ex 3
chemicals in a pond

10mil gal of water
water goes in 5 mil gal containing some chemical per year
 5 mil gal a year flows out 

photo in phone with pond


e^t/2 q is from [[Product Rule]]

## ex4
escape velocity

![[Pasted image 20230919110335.png]]
write down newtons second law f=ma
acceleration is [[derivative]] of velocity