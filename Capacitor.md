#physics #hardware 
**Definition:** Capacitors store and release electrical [[energy]] via two conductive plates separated by an insulating [[dielectric]] material.

**Key Points:**

- **[[Capacitance]] (C):** Measures the capacitor's ability to store charge, in Farads (F).
- **Charge and Discharge:** Capacitors accumulate and release charge when [[voltage]] is applied and removed.
- **[[Dielectric]]:** Insulating material between plates; influences capacitance and [[voltage]] ratings.
- **Types:** Electrolytic (polarized), Ceramic, Film, Tantalum, Supercapacitors.
- **Applications:** Smoothing [[voltage]], timing circuits, noise filtering, [[energy]] storage.

**Circuit Analysis Formulas with Capacitors:**

1. **Capacitance (C):**$$Q = C \times V$$
     - $Q$ is the charge stored in the capacitor (in Coulombs),
     - $C$ is the capacitance (in Farads),
     - $V$ is the [[voltage]] across the capacitor (in Volts).

2. **Capacitor Charging:**$$V(t) = V_0 \times (1 - e^{-\frac{t}{RC}})$$
     - $V(t)$ is the [[voltage]] across the capacitor at time $t$,
     - $V_0$ is the initial [[voltage]] across the capacitor,
     - $R$ is the resistance in the circuit (in Ohms),
     - $C$ is the capacitance (in Farads).

3. **Capacitor Discharging:**$$V(t) = V_0 \times e^{-\frac{t}{RC}}$$
     - $V(t)$ is the [[voltage]] across the capacitor at time $t$,
     - $V_0$ is the initial [[voltage]] across the capacitor,
     - $R$ is the resistance in the circuit (in Ohms),
     - $C$ is the capacitance (in Farads).

4. **Time Constant ($τ$):**$$τ = R \times C$$
     - $R$ is the resistance (in Ohms),
     - $C$ is the capacitance (in Farads).

5. **[[Current]] through the Capacitor (I):** $$I(t) = C \times \frac{dV(t)}{dt}$$
     - $I(t)$ is the [[current]] through the capacitor at time $t$ (in Amperes),
     - $C$ is the capacitance (in Farads),
     - $\frac{dV(t)}{dt}$ is the rate of change of [[voltage]] with respect to time (in Volts per second).

**Capacitors in Series:**

1. **Total Capacitance ($C_{\text{total}}$) in Series:**
   - $\frac{1}{C_{\text{total}}} = \frac{1}{C_1} + \frac{1}{C_2} + \frac{1}{C_3} + \ldots$
     - $C_{\text{total}}$ is the total capacitance when capacitors are connected in series (in Farads),
     - $C_1$, $C_2$, $C_3$, ... are the individual capacitances of capacitors in series (in Farads).

**Capacitors in Parallel:**

1. **Total Capacitance ($C_{\text{total}}$) in Parallel:**
   - $C_{\text{total}} = C_1 + C_2 + C_3 + \ldots$
     - $C_{\text{total}}$ is the total capacitance when capacitors are connected in parallel (in Farads),
     - $C_1$, $C_2$, $C_3$, ... are the individual capacitances of capacitors in parallel (in Farads).

**[[Voltage]] across Capacitors in Series:**

1. **[[Voltage]] across Capacitors in Series:**
   - The [[voltage]] across each capacitor in a series configuration is the same as the total [[voltage]] applied to the combination.

**Charge on Capacitors in Parallel:**

1. **Total Charge ($Q_{\text{total}}$) on Capacitors in Parallel:**
   - $Q_{\text{total}} = C_{\text{total}} \times V$
     - $Q_{\text{total}}$ is the total charge stored in capacitors in parallel (in Coulombs),
     - $C_{\text{total}}$ is the total capacitance (in Farads),
     - $V$ is the [[voltage]] applied across the capacitors (in Volts).

These formulas are essential for analyzing circuits with multiple capacitors connected in series or parallel configurations. Understanding these relationships is crucial for designing circuits with the desired capacitance values and [[voltage]] ratings.

**Tips:**

- **[[Polarity]]:** Electrolytic capacitors are polarized; mind the correct connections.
- **Discharge:** Capacitors retain charge; discharge safely before handling.
- No charge can pass through 
