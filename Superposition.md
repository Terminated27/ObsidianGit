# Differential equations
#math #diffeq 

# Circuit Analysis

#physics #hardware 
- [[Superposition]] is a fundamental principle in electrical circuit analysis.
- It states that in a [[linear circuit]] with multiple sources ([[voltage]] or [[current]]), the response ([[voltage]] or [[current]]) at any component is the algebraic sum of the individual responses caused by each source acting alone, with all other sources turned off.
- [[Superposition]] simplifies the analysis of complex circuits by breaking them down into simpler, solvable parts.
- To apply [[Superposition]], consider one source at a time while turning off all others (replacing [[voltage]] sources with [[short circuit]]s and [[current]] sources with [[open circuit]]s) and calculate the response for each source individually.
- Finally, combine the individual responses to find the overall response of the circuit.
- Superposition is applicable only in [[linear circuit]]s, where the response is directly proportional to the applied source ([[Ohm's Law]]), and it does not hold for nonlinear components like [[diode]]s and [[transistor]]s.
## How To Solve
1. replace original circuit [[Voltage Source]] with [[short circuit]]
2. establish a [[Ground]] reference
3. solve for desired [[Node Voltage]] using [[Node Method]], store as $e_1$


5. replace original circuit [[Current Source]] with [[open circuit]]
6. establish a [[Ground]] reference
7. solve for desired [[Node Voltage]] using [[Node Method]], store as $e_2$

8. [[voltage]] at [[node]] is equal to $e_1+e_2$
9. using $V=IR$ convert [[voltage]] to amperage if desired
![[Pasted image 20231010165302.png]]