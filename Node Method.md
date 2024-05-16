#math #physics #hardware 

typical convention is convert [[Branch Voltage]] to [[Node Voltage]]



### Easy Method

Establish All the [[Node]]s in the circuit

use [[Kirchhoff's Current Law]] with all lines going in as  with only [[resistor]] network
$$
\sum\frac{V_{in}-Node}{R}=0
$$
with [[capacitor]]
$$
i=c\frac{d}{dt}(V_{in}-Node)
$$
with [[inductor]] 
$$
i = i(0^+)+\frac{1}{L}\int_0^t(V_{in}-Node)dt
$$
direction of [[Current]] does not matter
![[Pasted image 20231010162258.png]]

For [[Voltage Source]] / [[Current Source]] you can also convert to [[Super Node]]
### Typical Notes
Advantages
- reduces number of variables
- [[Kirchhoff's Voltage Law]] - is self satisfied
	- no longer need to worry about KVL anymore, its always 0 
![[Pasted image 20230922091327.png]]

1. ground one of the nodes and label the other nodes (Define a reference)
2. label the nodes & voltages, some can be unknown
	1. e1 = v1 & v2 & v5
	2. e2 = v2 & v3
	3. e3 = v3 & v4 & v5
3. start calculating nodes using [[Kirchhoff's Current Law]]
	1. $V_1 = e_1$ the positive terminal
	2. $V_2 = e_2-e_1$
	3. $V_3=e_3-e_2$
	4. $V_4=e_3$
	5. $V_5=e_3-e_1$
4. Solve Equations