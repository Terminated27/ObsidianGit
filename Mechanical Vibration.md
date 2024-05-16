# Differential Equations
#math #diffeq 
![[Pasted image 20231024103344.png]]
(1) = [[Hooke's law]]
(2) = mg

Mechanical vibrations are oscillatory motions of mechanical systems. These vibrations are pervasive in engineering and nature, from the oscillation of bridges due to wind to the motion of atoms in a molecule. Understanding and analyzing mechanical vibrations are crucial for designing stable structures and predicting system behavior.

**Modeling Mechanical Vibrations:**

Mechanical vibrations are often modeled using second-[[order]] [[linear]] ordinary differential equations (ODEs) derived from Newton's second law of motion.

**Basic Equation:**
$$m \frac{d^2x}{dt^2} + c \frac{dx}{dt} + kx = 0$$

Where:
- $m$ is the mass of the vibrating object (in kg).
- $x(t)$ is the displacement of the object from its equilibrium position at time $t$ (in meters, m).
- $c$ is the damping coefficient, which represents the damping or resistance to motion (in kg/s).
- $k$ is the stiffness of the system, representing how stiff the system is (in N/m).
- $\frac{d^2x}{dt^2}$ represents the acceleration of the object.

**Solutions to the [[Differential Equation]]: Use [[Non-homogeneous second order ODE with constant coefficients]]**

1. **Undamped Free Vibration (No Damping - $c = 0$):**
$$m \frac{d^2x}{dt^2} + kx = 0$$
Solutions are sinusoidal functions: $x(t) = A \sin(\omega t + \phi)$, where $\omega = \sqrt{\frac{k}{m}}$ is the angular frequency, $A$ is the amplitude, and $\phi$ is the [[phase angle]].

2. **Damped Free Vibration ($c > 0$):**
$$m \frac{d^2x}{dt^2} + c \frac{dx}{dt} + kx = 0$$
Solutions involve exponential decay: $x(t) = Ae^{-\frac{c}{2m}t} \cos(\sqrt{\frac{k}{m} - \left(\frac{c}{2m}\right)^2}t + \phi)$.

3. **[[Forced Vibration]] ($F(t) \neq 0$):**
$$m \frac{d^2x}{dt^2} + c \frac{dx}{dt} + kx = F(t)$$
The solution depends on the specific form of the applied force $F(t)$ and often involves solving the equation using methods like undetermined coefficients or Laplace transforms.

if having trouble graphing, use some [[Sin Identities]] to simplify