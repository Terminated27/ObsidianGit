#math #diffeq #computing 
Use computer to draw the graph of a solution to an [[ODE]]

1. start from [[initial condition]]
2. Determine the [[Mesh Size]] $h\approx 0$ 
	we can use approximate 
	if $t_1\approx t_2$ 
	$y(t_2)\approx y(t_1)+\frac{dy}{dt}t_1*(t_1-t_2)$ 
	$\hookrightarrow$ [[linear approximation]] from [[Taylor series]]
3. compute $y(t_n)=y(t_{n-1})+h_0f(t_{n-1}y(t_{n-1}))$
4. repeat until $t_n>T$

to graph accurately, make T small and $h_0$ small too