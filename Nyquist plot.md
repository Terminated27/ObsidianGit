![[Pasted image 20240325103953.png]]
A Nyquist plot is a graphical representation of the frequency response of a system in the complex plane. It is commonly used in control systems analysis to study the stability and performance of a system.

## Key Theorems and Definitions

1. **Nyquist Stability Criterion**: The Nyquist stability criterion states that a system is stable if and only if the Nyquist plot encircles the point (-1,0) in the counterclockwise direction exactly N times, where N is the number of poles of the [[transfer function]] located in the right half of the complex plane.

2. **Nyquist Frequency**: The frequency at which the Nyquist plot intersects the negative real axis is known as the Nyquist frequency. It corresponds to the crossover frequency in Bode plots.

## Step-by-Step Example

Consider a [[transfer function]] $G(s)$ with poles at $s = -1$ and $s = -2$, and no zeros. The Nyquist plot can be obtained by evaluating $G(j\omega)$ for $\omega \in [0, \infty)$.

1. At $\omega = 0$, $G(j\omega) = G(0)$. Since there are no zeros, this point lies on the real axis.
2. As $\omega$ increases, we evaluate $G(j\omega)$ at each frequency and plot these points in the complex plane.
3. The Nyquist plot will start from $G(0)$ and approach infinity as $\omega$ approaches infinity.
4. The plot will encircle (-1,0) once counterclockwise due to one pole in the right half plane at $s=-1$.
5. If there were more poles or zeros, additional encirclements would occur based on their locations.

By analyzing the Nyquist plot, we can determine stability and gain margins of a system without explicitly solving for poles or zeros.

In conclusion, Nyquist plots provide valuable insights into system behavior and stability through graphical representation in the complex plane. Understanding key concepts such as Nyquist stability criterion and Nyquist frequency is essential for control systems analysis using this powerful tool.