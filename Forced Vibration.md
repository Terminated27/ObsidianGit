#physics #math #diffeq 

**A. Particular Solution for Various External Forces:**

1. **Sinusoidal Force:** When the external force $F(t)$ is sinusoidal ($F(t) = F_0 \sin(\omega t)$), the particular solution can be assumed to have the same form. For a system with damping ($c > 0$), the amplitude and [[phase]] angle are determined using the complex representation of the equation.

$$ x_p(t) = \frac{F_0}{\sqrt{(k - m\omega^2)^2 + (c\omega)^2}} \sin(\omega t - \phi) $$

2. **[[Step Function]] Force:** When the external force is a [[step function]], the equation of motion changes instantaneously. Solving this equation requires considering different cases based on the time at which the [[step function]] occurs.

3. **Impulse Force:** An impulse force ($F(t) = \delta(t - t_0)$) represents an instantaneous application of force. The solution involves integrating the equation of motion over a small time interval around $t_0$, considering the impulse force as the limit of a very short-duration force.

**B. [[Frequency Response Function]]:**

The [[frequency response function]] (FRF) is a vital concept in forced vibration analysis. It quantifies the system's response amplitude at a specific frequency of the external force. For a sinusoidal force, the FRF is given by:

$$ H(\omega) = \frac{X(\omega)}{F_0} = \frac{1}{\sqrt{(k - m\omega^2)^2 + (c\omega)^2}} $$

This function illustrates how the system amplifies or attenuates the input amplitude at different frequencies. Resonance occurs at the natural frequency ($\omega = \omega_0$) where $|H(\omega)|$ is maximized.

**C. Complex Notation and Phasors:**

Complex notation is often employed to simplify the mathematics of forced vibration problems. By representing the displacement, velocity, and force in complex form ($X e^{i\phi}$), the differential equations transform into algebraic equations. Phasors, which are rotating vectors representing complex amplitudes, provide a geometric understanding of the [[phase]] relationships between displacement, velocity, and force in forced vibration problems.

**D. Damping and Its Effects:**

Damping significantly influences forced vibration behavior. Damping not only attenuates the amplitude of vibration but also introduces [[phase]] shifts between the force and response. This [[phase]] shift can lead to interesting phenomena, such as the lagging of the response behind the force in underdamped systems.

## Variables used

1. **$m$**: Mass of the system. It represents the amount of matter in the object undergoing vibration.

2. **$c$**: Damping coefficient. Damping is a force that opposes the motion of an object, and the damping coefficient quantifies this force. Higher damping coefficients indicate more damping and quicker dissipation of [[energy]].

3. **$k$**: Stiffness of the system. It characterizes how stiff or compliant the system is. High stiffness means the system is resistant to deformation.

4. **$x(t)$**: Displacement of the system from its equilibrium position at time $t$. It represents how far the system has moved from its rest position at any given time.

5. **$F(t)$**: External force applied to the system as a function of time $t$. This force can vary in magnitude and direction and is the cause of the vibration.

6. **$\omega$**: Angular frequency of the external force. It is related to the frequency ($f$) of the force by the equation $\omega = 2\pi f$. Angular frequency represents how rapidly the force oscillates.

7. **$X$**: Amplitude of the forced vibration. It represents the maximum displacement of the system from its equilibrium position in response to the external force.

8. **$\phi$**: [[Phase angle]]. It represents the [[phase]] shift between the external force and the system's response. It determines the position of the vibration relative to the force's cycle.

9. **$\delta(t - t_0)$**: Impulse force applied to the system at a specific time $t_0$. An impulse force is a very short-duration force applied instantaneously.

10. **$\frac{d^2x}{dt^2}$**: Second [[Derivative]] of displacement with respect to time. It represents acceleration, indicating how quickly the velocity of the system is changing.

11. **$\frac{dx}{dt}$**: First [[Derivative]] of displacement with respect to time. It represents velocity, indicating how quickly the position of the system is changing.

12. **$F_0$**: Amplitude or peak value of the external force applied to the system. It represents the maximum magnitude of the force and does not specify a particular time $t$ at which the force is applied. Instead, it quantifies the force's maximum intensity during the entire vibration process.