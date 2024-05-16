#hardware #math #physics 

The Shockley diode equation, also known as the [[diode current equation]], is a mathematical model that describes the [[current]]-[[voltage]] relationship in a semiconductor diode. It was developed by William Shockley, one of the inventors of the transistor.

## Equation Formulation

The Shockley diode equation relates the [[current]] flowing through a diode to the [[voltage]] across it. It is given by:

$$I_D = I_S \left( e^{\frac{V_D}{nV_T}} - 1 \right)$$

where:
- $I_D$ is the diode [[current]],
- $I_S$ is the [[reverse saturation current]],
- $V_D$ is the [[voltage]] across the diode,
- $n$ is the ideality factor, and
- $V_T$ is the [[thermal voltage]].

## Key Definitions

1. **[[Reverse Saturation Current]] ($I_S$)**: The reverse saturation [[current]] represents the small amount of [[current]] that flows through a diode when it is reverse biased. It depends on factors such as temperature and material properties.

2. **Ideality Factor ($n$)**: The ideality factor accounts for deviations from ideal behavior in a real diode. It takes into consideration factors like recombination and series resistance. In an ideal diode, $n = 1$, but in practice, it can have values between 1 and 2.

3. **Thermal [[Voltage]] ($V_T$)**: The thermal [[voltage]] represents the [[energy]] associated with each electron at a given temperature. It is given by:

   $$V_T = \frac{kT}{q}$$
   
   where:
   - $k$ is Boltzmann's constant,
   - $T$ is absolute temperature in Kelvin, and
   - $q$ is electron charge.

## Example

Let's consider an example to illustrate the application of the Shockley diode equation.

Suppose we have a silicon diode with a reverse saturation [[current]] of $I_S = 10^{-12}$ A and an ideality factor of $n = 1.5$. We want to find the diode [[current]] for a forward [[voltage]] of $V_D = 0.7$ V at room temperature ($T = 300$ K).

First, we calculate the thermal [[voltage]]:

$$V_T = \frac{kT}{q} = \frac{(1.38 \times 10^{-23} \, \text{J/K})(300 \, \text{K})}{1.6 \times 10^{-19} \, \text{C}}$$

Next, we substitute the given values into the Shockley diode equation:

$$I_D = (10^{-12} \, \text{A})\left(e^{\frac{0.7}{1.5V_T}} - 1\right)$$

Finally, we can solve this equation to find the diode [[current]].

## Conclusion

The Shockley diode equation provides a mathematical model for understanding the behavior of semiconductor diodes. It allows us to analyze and predict the [[current]]-[[voltage]] characteristics of diodes under different operating conditions. By considering factors such as reverse saturation [[current]] and ideality factor, this equation provides valuable insights into diode behavior in practical circuits.