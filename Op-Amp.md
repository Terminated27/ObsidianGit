#physics #hardware 

**Operational Amplifiers (Op-Amps) in Circuit Analysis**
[[identifying op-amp]]
**1. Definition:**
An [[op-amp]] amplifies the difference in [[voltage]] between its two input terminals (inverting and non-inverting) and produces a corresponding output [[voltage]]

The key formula related to the ideal behavior of an [[op-amp]] is the virtual short-circuit equation, which states that the [[voltage]] at the inverting (-) and non-inverting (+) input terminals of the [[op-amp]] are virtually equal:

$V_+-V_-=0$

**2. Ideal
Properties:**
- Infinite open-loop [[voltage]] gain ($(A_{{OL}}$)).
- Infinite input [[impedance]] ($(Z_{{in}} = \infty$)).
- Zero output [[impedance]] ($(Z_{{out}} = 0$)).
- Infinite bandwidth.
- Zero input offset [[voltage]] ($(V_{{os}} = 0$)).
- Infinite common-mode rejection ratio (CMRR).

**3. Inverting Amplifier:**
The basic inverting amplifier configuration is given by the following equation:
$$V_{{out}} = -(\frac{R_f}{R_{{in}}}) \times V_{{in}}$$

Where ( $R_f$) is the feedback [[resistor]] and ($R_{{in}}$) is the input [[resistor]].

**4. Non-Inverting Amplifier:**
The non-inverting amplifier configuration is given by:$$V_{out} = (1 + \frac{R_f}{R_{{in}}}) * V_{{in}}$$

**5. Summing Amplifier:**
For a summing amplifier with ( $n$ ) inputs:
$$V_{{out}} = -(\frac{R_f}{R_1} \times V_1 + \frac{R_f}{R_2} \times V_2 + \ldots + \frac{R_f}{R_n} \times V_n)$$

**6. Difference Amplifier:**
For a difference amplifier:
$$V_{out}=(\frac{R_f}{R_1}\times V_1 - \frac{R_f}{R_1}\times V_2)$$

**7. Integrator:**
For an [[op-amp]] integrator circuit, the output [[voltage]] is the [[integral]] of the input [[voltage]]:
$$V_{out}(t) = \frac{1}{R_f\times C}\int V_{in}(t)dt$$

Where ( $R_f$) is the feedback [[resistor]] and ( $C$) is the [[capacitor]] value.

**8. Differentiator:**
For an [[op-amp]] differentiator circuit, the output [[voltage]] is the [[Derivative]] of the input [[voltage]]:
$$V_{out}(t) = -R_f \times C \times \frac{d}{dt}V_{in}(t)$$

**9. Slew Rate (SR):**
Slew rate is the maximum rate of change of output [[voltage]] per unit of time and is expressed in V/µs.
$$Slew Rate = \frac{\Delta V_{out}}{\Delta t}$$

Where ( $\Delta V_{{out}}$) is the change in output [[voltage]] and ( $\Delta t$) is the corresponding time interval.

### Circuit analysis
