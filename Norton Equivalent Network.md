#physics #hardware #math 
similar to [[Thevenin Equivalent Network]]
### Norton Equivalent Circuit:

The Norton Equivalent Circuit is a simplification technique in electrical engineering used to analyze complex networks. It allows you to replace a portion of a circuit with a single [[current source]] in parallel with a single [[resistor]]. This simplifies the circuit analysis without changing the external behavior of the original circuit.

### Components of Norton Equivalent Circuit:

1. **[[Current Source]] (I_n):** Represents the total [[current]] flowing out of the equivalent circuit.
   
2. **Resistance (R_n):** Represents the [[equivalent resistance]] of the circuit as seen from the terminals where the Norton Equivalent is derived.

### Steps to Find Norton Equivalent:

1. **Identify Load:** Choose a part of the circuit where you want to know the equivalent.
2. **Remove Load:** Temporarily take out the component.
3. **Short Circuit:** short the open terminals
4. **Find $I_{n}$:** Calculate the [[current]] at the shorted terminals.
5. **Find $R_{n}$​:** Determine the [[resistance]] looking back into the shorted terminals with all sources turned off.

![[Pasted image 20231012210928.png]]