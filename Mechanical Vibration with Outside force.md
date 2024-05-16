#physics #diffeq #math 

[[Mechanical vibration]] refers to the rapid oscillatory motion of an object around an equilibrium position. When subjected to external forces, the analysis of mechanical vibrations becomes intricate, often requiring the use of differential equations. This atomic note explores the fundamental aspects of [[mechanical vibration]] under external forces, with a specific emphasis on the differential equations governing this phenomenon.

**I. Free Vibration:**
In the absence of external forces, mechanical systems exhibit free vibration. For a single-degree-of-freedom system, the equation of motion can be represented as:

$$m \frac{d^2x}{dt^2} + c \frac{dx}{dt} + kx = 0 $$

Where:
- $m$ is the mass of the system,
- $c$ is the damping coefficient,
- $k$ is the stiffness of the system,
- $x$ is the displacement from equilibrium.

**II. [[Forced Vibration]]:**
When an external force $F(t)$ is applied to the system, the equation of motion becomes:

$$m \frac{d^2x}{dt^2} + c \frac{dx}{dt} + kx = F(t) $$

**III. Solving the [[Differential Equation]]:**
The solution to the [[forced vibration]] equation involves finding the particular solution and the complementary function. The particular solution depends on the form of the external force $F(t)$ (e.g., sinusoidal, [[step function]], impulse). The complementary function represents the natural response of the system (free vibration).

**IV. Harmonic External Force:**
For a sinusoidal external force $F(t) = F_0 \sin(\omega t)$, the particular solution can be assumed to have the same form as the external force, leading to the equation:

$$x_p(t) = X \sin(\omega t - \phi) $$

Where $X$ is the amplitude of the [[forced vibration]], and $\phi$ is the [[phase]] angle.

**V. Resonance:**
Resonance occurs when the frequency of the external force matches the natural frequency of the system ($\omega = \omega_0$). In such cases, the amplitude of vibration becomes unbounded, emphasizing the importance of understanding [[forced vibration]] dynamics.

**VI. Conclusion:**
The study of [[mechanical vibration]] with external forces is crucial in various engineering applications. Differential equations serve as powerful tools in analyzing and predicting the behavior of mechanical systems subjected to external forces. By understanding the interplay between the external forces and the inherent characteristics of the system, engineers can design systems that are resilient and efficient in real-world scenarios.

[[Damping Ratio]]