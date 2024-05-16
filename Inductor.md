#physics #hardware 

Inductors are passive electronic components that store [[energy]] in the form of a magnetic field when an electric [[current]] flows through them. They consist of a coil of wire, often wound around a core made of ferrous material. Inductors resist changes in [[current]], causing the [[current]] to lag behind the [[voltage]] in AC circuits. They are widely used in electronic circuits for various purposes, including [[energy]] storage, filtering, and signal processing. Inductors are represented by the symbol L in circuit diagrams and are measured in Henrys (H). Understanding the behavior of inductors and their interaction with other components is essential for designing and analyzing complex electrical circuits.


**Circuit Analysis Formulas with Inductors:**

1. **Inductance ($L$):**$$V = L \times \frac{di}{dt}$$
     - $V$ is the [[voltage]] across the inductor (in Volts),
     - $L$ is the inductance (in Henrys),
     - $\frac{di}{dt}$ is the rate of change of [[current]] with respect to time (in Amperes per second).

2. **Inductor [[Current]] in DC Circuits:**$$V = L \times I$$
     - $V$ is the [[voltage]] across the inductor (in Volts),
     - $L$ is the inductance (in Henrys),
     - $I$ is the [[current]] through the inductor (in Amperes).

3. **Inductor [[Current]] in AC Circuits:**$$V = L \times \frac{dI}{dt}$$
     - $V$ is the instantaneous [[voltage]] across the inductor (in Volts),
     - $L$ is the inductance (in Henrys),
     - $\frac{dI}{dt}$ is the [[Derivative]] of [[current]] with respect to time (in Amperes per second).

4. **Inductive Reactance ($X_L$) in AC Circuits:**$$X_L = 2\pi fL$$
     - $X_L$ is the inductive reactance (in Ohms),
     - $f$ is the frequency of the alternating [[current]] (in Hertz),
     - $L$ is the inductance (in Henrys).

The average [[current]] ($I_{\text{avg}}$) flowing through an inductor ($L$) over a specific time interval $[t_1, t_2]$ can be calculated using the formula:

$$ I_{\text{avg}} = \frac{1}{L} \int_{t_1}^{t_2} V(t) \, dt $$

- \(L\) is the inductance of the inductor in henries (H).
- \(V(t)\) is the [[voltage]] across the inductor as a function of time, measured in volts (V).
- \(t\) represents time in seconds (s).

This formula represents the average [[current]] obtained by integrating the [[voltage]] function \(V(t)\) over the specified time interval and dividing the result by the inductance \(L\).

5. **[[Energy]] Stored in an Inductor:**$$W = \frac{1}{2} L I^2$$
     - $W$ is the [[energy]] stored in the inductor (in Joules),
     - $L$ is the inductance (in Henrys),
     - $I$ is the [[current]] through the inductor (in Amperes).

**Inductors in Series:**

 **Total Inductance ($L_{\text{total}}$) in Series:**$$\frac{1}{L_{\text{total}}} = \frac{1}{L_1} + \frac{1}{L_2} + \frac{1}{L_3} + \ldots$$
     - $L_{\text{total}}$ is the total inductance when inductors are connected in series (in Henrys),
     - $L_1$, $L_2$, $L_3$, ... are the individual inductances of inductors in series (in Henrys).

**Inductors in Parallel:**

 **Total Inductance ($L_{\text{total}}$) in Parallel:**$$L_{\text{total}} = L_1 + L_2 + L_3 + \ldots$$
     - $L_{\text{total}}$ is the total inductance when inductors are connected in parallel (in Henrys),
     - $L_1$, $L_2$, $L_3$, ... are the individual inductances of inductors in parallel (in Henrys).

**[[Impedance]] in Series (for AC Circuits):**

 **Total [[Impedance]] ($Z_{\text{total}}$) in Series:**$$Z_{\text{total}} = j\omega L_{\text{total}}$$
     - $Z_{\text{total}}$ is the total [[impedance]] in a series inductive circuit (in Ohms),
     - $j$ is the imaginary unit ($j^2 = -1$),
     - $\omega$ is the angular frequency of the AC circuit (in radians per second),
     - $L_{\text{total}}$ is the total inductance in the series circuit (in Henrys).

**[[Impedance]] in Parallel (for AC Circuits):**


 **Total [[Impedance]] ($Z_{\text{total}}$) in Parallel:**$$\frac{1}{Z_{\text{total}}} = \frac{1}{j\omega L_1} + \frac{1}{j\omega L_2} + \frac{1}{j\omega L_3} + \ldots$$
     - $Z_{\text{total}}$ is the total [[impedance]] in a parallel inductive circuit (in Ohms),
     - $j$ is the imaginary unit ($j^2 = -1$),
     - $\omega$ is the angular frequency of the AC circuit (in radians per second),
     - $L_1$, $L_2$, $L_3$, ... are the individual inductances of inductors in parallel (in Henrys).
