#hardware 

In the field of Circuits and Electronics, CMOS (Complementary Metal-Oxide-Semiconductor) technology plays a crucial role in the design and analysis of digital circuits. One important aspect of CMOS circuits is their delay, which refers to the time it takes for a signal to propagate through the circuit. Understanding CMOS delay is essential for designing efficient and reliable digital systems.

## Introduction to CMOS Delay

CMOS delay is primarily determined by two factors: **[[capacitance]]** and **resistance**. [[Capacitance]] represents the ability of a component or wire to store charge, while resistance measures its opposition to the flow of [[current]]. In CMOS circuits, [[capacitance]] arises from various sources such as gate [[capacitance]], interconnect [[capacitance]], and [[load capacitance]]. Resistance mainly comes from the transistor channel resistance and interconnect resistance.

The delay in a CMOS circuit can be divided into two components: **[[intrinsic delay]]** and **extrinsic delay**. The [[intrinsic delay]] is caused by the transistor switching characteristics, while the extrinsic delay is due to the interconnects and [[load capacitance]].

## [[Intrinsic Delay]]

The [[intrinsic delay]] in a CMOS circuit primarily depends on three factors: **transistor sizing**, **[[transistor threshold voltage]]**, and **input transition time**.

### Transistor Sizing

Transistor sizing refers to adjusting the width-to-length ratio (W/L) of transistors in a circuit. By changing this ratio, we can control the strength of each transistor. In general, larger transistors have lower resistance but higher [[capacitance]], leading to slower switching times. Conversely, smaller transistors have higher resistance but lower [[capacitance]], resulting in faster switching times.

### Transistor Threshold [[Voltage]]

The threshold [[voltage]] (Vth) of a transistor determines when it turns on or off. A lower threshold [[voltage]] leads to faster switching times, as the transistor becomes conductive at a lower input [[voltage]]. However, reducing the threshold [[voltage]] also increases leakage [[current]], which can negatively impact [[power]] consumption.

### Input Transition Time

The input transition time (τ) is the time it takes for the input signal to transition from one logic level to another. A shorter transition time results in faster switching speeds and reduced delay.

## Extrinsic Delay

The extrinsic delay in a CMOS circuit is mainly determined by [[interconnect capacitance]] and [[load capacitance]].

### [[Interconnect Capacitance]]

[[Interconnect capacitance]] arises from the wires used to connect different components in a circuit. As signals propagate through these wires, they experience a delay due to the [[capacitance]] of the wires. The longer and narrower the wires, the higher their resistance and [[capacitance]], leading to increased delay.

### [[Load Capacitance]]

[[Load capacitance]] represents the total [[capacitance]] seen by an output [[node]] of a CMOS gate. It includes both the intrinsic gate [[capacitance]] and any additional [[capacitance]] connected to the output [[node]]. The larger the [[load capacitance]], the longer it takes for an output signal to reach its final value.

## Delay Calculation

To calculate the total delay in a CMOS circuit, we need to consider both intrinsic and extrinsic delays. The total delay ($T_{delay}$) can be expressed as:

$$T_{\text{delay}} = T_{\text{intrinsic}} + T_{\text{extrinsic}}$$

The [[intrinsic delay]] ($T_{intrinsic}$) can be further divided into two components: **rise delay** ($T_{rise}$) and **fall delay** ($T_{fall}$). These delays represent how long it takes for an output signal to rise or fall from 10% to 90% of its final value (in this class we find for 50%).

$$T_{\text{intrinsic}} = T_{\text{rise}} + T_{\text{fall}}$$

The [[extrinsic delay]] ($T_{extrinsic}$) is primarily determined by the [[load capacitance]] ($C_{load}$) and the resistance (R) of the interconnects. It can be calculated using the following formula:

$$T_{\text{extrinsic}} = R \cdot C_{\text{load}}$$

## Example Circuit Analysis

Let's consider a simple CMOS inverter circuit as an example to illustrate the calculation of delay.
![[Pasted image 20231113093418.png]]
Assume that the transistor sizing, threshold [[voltage]], input transition time, [[interconnect capacitance]], and [[load capacitance]] are known for this circuit. We want to calculate the total delay.

Given:
- Transistor sizing: W/L = 2
- Threshold [[voltage]]: Vth = 0.5V
- Input transition time: τ = 1ns
- Interconnect resistance: R = 100Ω
- [[Load capacitance]]: Cload = 10pF

First, we calculate the [[intrinsic delay]] using the rise and fall delays:

$$T_{\text{rise}} = \frac{{0.69 \cdot W/L}}{{V_{\text{dd}} - V_{\text{th}}}} \cdot C_{\text{intrinsic}}$$

$$T_{\text{fall}} = \frac{{0.69 \cdot W/L}}{{V_{\text{dd}} - V_{\text{th}}}} \cdot C_{\text{intrinsic}}$$

Next, we calculate the [[extrinsic delay]] using the interconnect resistance and [[load capacitance]]:

$$T_{\text{extrinsic}} = R \cdot C_{\text{load}}$$

Finally, we obtain the total delay ([[Propagation Delay]]) by summing the intrinsic and extrinsic delays:

$$T_{\text{delay}} = T_{\text{intrinsic}} + T_{\text{extrinsic}}$$

By substituting the given values into these equations, we can calculate the delay for this specific CMOS inverter circuit.

## Conclusion

CMOS delay is a critical aspect of digital circuit analysis. By understanding the factors that contribute to delay, such as transistor sizing, threshold [[voltage]], and [[capacitance]], we can design more efficient and reliable digital systems. The calculation of delay involves considering both intrinsic and extrinsic delays, which can be determined using appropriate formulas. Through comprehensive circuit analysis examples like the CMOS inverter circuit discussed above, we can gain a deeper understanding of CMOS delay and its implications in Circuits and Electronics 1.