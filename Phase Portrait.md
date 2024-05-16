
#math #diffeq 
A [[phase]] portrait is a graphical representation of the behavior of a dynamical system in the [[phase]] space. It provides a visual understanding of how the system's state evolves over time. In this atomic note, we will explore the concept of [[phase]] portraits and their significance in analyzing dynamical systems.

1. **Saddle Point:**
   - *Description:* Equilibrium point where trajectories move away in some directions and toward in others.
   - *Eigenvalues:* Real, with opposite signs.

2. **[[Node]] (or Sink):**
   - *Description:* Stable equilibrium where trajectories converge towards the point.
   - *Eigenvalues:* Real, both negative.

3. **Source:**
   - *Description:* Unstable equilibrium where trajectories diverge away from the point.
   - *Eigenvalues:* Real, both positive.

4. **Center:**
   - *Description:* Stable equilibrium with trajectories circulating around the point.
   - *Eigenvalues:* Complex conjugates with zero real part.

5. **Spiral Source:**
   - *Description:* Unstable equilibrium with outward spiraling trajectories.
   - *Eigenvalues:* Complex conjugates with positive real part.

6. **Spiral Sink:**
   - *Description:* Stable equilibrium with inward spiraling trajectories.
   - *Eigenvalues:* Complex conjugates with negative real part.
 

![[Pasted image 20231128135118.png]]
## Definition

A [[phase]] portrait is a plot of representative trajectories of a dynamical system in the [[phase]] space. The [[phase]] space is a mathematical space where each point represents a unique state of the system. For example, consider a simple [[linear differential]] equation:

$$\frac{{dx}}{{dt}} = ax$$

where $x$ is the state variable and $a$ is a constant. The [[phase]] portrait for this system would be a plot of $x$ versus $t$, showing how the state variable evolves over time.

## Equilibrium Points

Equilibrium points play a crucial role in understanding [[phase]] portraits. An equilibrium point, also known as a critical point or fixed point, is a state where the [[Derivative]] of the system with respect to time is zero. Mathematically, for a dynamical system $\frac{{dx}}{{dt}} = f(x)$, an equilibrium point occurs when $f(x) = 0$.

The behavior of trajectories near equilibrium points provides valuable information about stability and attractivity of these points. There are three types of equilibrium points:

1. **Stable Equilibrium**: Trajectories near stable equilibrium points converge towards them as time progresses.
2. **Unstable Equilibrium**: Trajectories near unstable equilibrium points diverge away from them as time progresses.
3. **Semi-Stable Equilibrium**: Trajectories on one side converge towards semi-stable equilibrium points, while on the other side they diverge away.

## [[Phase]] Portraits for Linear Systems

Linear systems are particularly interesting due to their simplicity and well-understood behavior. Consider a linear [[autonomous system]]:

$$\frac{{d\mathbf{x}}}{{dt}} = \mathbf{Ax}$$

where $\mathbf{x}$ is a vector of state variables and $\mathbf{A}$ is a constant matrix. The [[phase]] portrait for this system can be obtained by analyzing the [[Eigenvalues]] and [[eigenvectors]] of $\mathbf{A}$.

If all [[Eigenvalues]] have negative real parts, the equilibrium point at the origin is stable, and trajectories converge towards it. If all [[Eigenvalues]] have positive real parts, the origin is unstable, and trajectories diverge away from it. If some [[Eigenvalues]] have negative real parts while others have positive real parts, semi-stable equilibrium points exist.

## Example: Simple Harmonic Oscillator

Let's consider a simple harmonic oscillator described by the following second-order [[Differential Equation]]:

$$\frac{{d^2x}}{{dt^2}} + \omega^2 x = 0$$

where $x$ represents the displacement from equilibrium and $\omega$ is the angular frequency.

To convert this second-order equation into a system of first-order equations, we introduce a new variable $v = \frac{{dx}}{{dt}}$, representing velocity. Now we have:

$$\frac{{dx}}{{dt}} = v$$
$$\frac{{dv}}{{dt}} = -\omega^2 x$$

This system can be written in matrix form as:

$$\frac{{d\mathbf{x}}}{{dt}} = \begin{bmatrix} 0 & 1 \\ -\omega^2 & 0 \end{bmatrix} \mathbf{x}$$

The [[Eigenvalues]] of this matrix are $\pm i\omega$, which have zero real parts. Therefore, the origin (equilibrium point) is semi-stable. Trajectories in [[phase]] space form ellipses around the origin.

## Conclusion

[[Phase]] portraits provide valuable insights into the behavior of dynamical systems. By analyzing the equilibrium points and their stability, we can understand the long-term evolution of the system. Linear systems can be analyzed using [[Eigenvalues]] and [[eigenvectors]], while [[non-linear]] systems often require numerical methods for [[phase]] portrait analysis.