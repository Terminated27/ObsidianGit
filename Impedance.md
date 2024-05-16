
In the context of continuous time signals, impedance plays a crucial role in understanding the behavior of electrical circuits. Impedance ($Z$) is a complex quantity that characterizes how a circuit responds to sinusoidal input signals. It is defined as the ratio of phasor [[voltage]] ($\tilde{V}$) to phasor current ($\tilde{I}$) in a circuit:

$$ Z = \frac{\tilde{V}}{\tilde{I}} $$

Impedance can be represented in terms of resistance ($R$), inductance ($L$), and capacitance ($C$) as follows:

- For a [[resistor]] with resistance $R$, the impedance is equal to the resistance itself: $Z_R = R$
- For an [[inductor]] with inductance $L$, the impedance is given by: $Z_L = j\omega L$
- For a capacitor with capacitance $C$, the impedance is: $Z_C = \frac{1}{j\omega C}$

where $\omega$ represents the angular frequency of the input signal.

## Key Theorems and Definitions

### [[Ohm's Law]] for AC Circuits
[[Ohm's Law]] for AC circuits relates [[voltage]], [[current]], and impedance:
$$ \tilde{V} = Z \cdot \tilde{I} $$

### Impedance Matching
Impedance matching is essential for maximum [[power]] transfer between components. It occurs when the load impedance matches the source impedance.

## Step-by-Step Example

Consider a series RL circuit with a [[resistor]] of 10 ohms and an [[inductor]] with an inductance of 2 H. If a sinusoidal [[voltage]] source with amplitude 5 V and frequency 50 Hz is applied to this circuit, calculate the total impedance.

Given:
- Resistance, $R = 10 \Omega$
- Inductance, $L = 2 H$
- Angular frequency, $\omega = 2\pi f = 100\pi$

The total impedance can be calculated as:
$$ Z_{\text{total}} = R + j\omega L = 10 + j200\pi $$

Therefore, the total impedance of the series RL circuit is $10 + j200\pi \Omega$.