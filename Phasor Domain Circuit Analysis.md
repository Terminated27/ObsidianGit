

# Phasor Domain Circuit Analysis

Phasor domain circuit analysis is a powerful technique used to analyze AC circuits by representing sinusoidal signals as complex numbers called phasors. This method simplifies the analysis of circuits with multiple components and varying frequencies.

## Key Theorems and Definitions

### Phasor Representation
In phasor domain analysis, a sinusoidal signal $v(t) = V_m \cos(\omega t + \phi)$ can be represented as a phasor $\underline{V} = V_m \angle \phi$, where $V_m$ is the magnitude of the signal and $\phi$ is the [[phase angle]].

### [[Impedance]]
[[Impedance]] is the complex resistance in AC circuits, denoted by $Z$. For a [[resistor]] with resistance $R$, [[inductor]] with inductance $L$, and capacitor with capacitance $C$, their impedances are given by:
- [[Resistor]]: $Z_R = R$
- [[Inductor]]: $Z_L = j\omega L$
- Capacitor: $Z_C = \frac{1}{j\omega C}$

### Kirchhoff's Laws in Phasor Domain
[[Kirchhoff's voltage law]] (KVL) and [[Kirchhoff's current law]] (KCL) can be applied in the phasor domain by summing voltages and currents around loops and nodes, respectively.

## Step-by-Step Example

Consider a series RL circuit with a [[voltage]] source $V_s$ connected to a [[resistor]] $R$ and an [[inductor]] $L$. The circuit can be represented in the phasor domain as follows:

$$\underline{V}_s = \underline{I}(R + j\omega L)$$

To solve for the [[current]] $\underline{I}$ flowing through the circuit, we can use [[Ohm's law]]:

$$\underline{I} = \frac{\underline{V}_s}{R + j\omega L}$$

Substitute $\underline{V}_s = V_s \angle 0^\circ$ into the equation above to find the current phasor $\underline{I}$. Finally, convert $\underline{I}$ back to time domain to obtain the sinusoidal [[current]] waveform.

Phasor domain circuit analysis simplifies complex calculations involving AC circuits and provides insights into circuit behavior under varying frequency conditions. By leveraging phasors, engineers can efficiently analyze and design electrical systems for optimal performance.