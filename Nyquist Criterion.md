The Nyquist criterion is a fundamental concept in control theory that is used to analyze the stability of a system based on its frequency response. It is named after Harry Nyquist, who introduced the criterion in the 1930s.

## Key Theorems and Definitions

### Nyquist Stability Criterion

The Nyquist stability criterion states that a system is stable if and only if the [[Nyquist plot]] of its [[transfer function]] encircles the point (-1,0) in the complex plane in a counterclockwise direction exactly N times, where N is the number of poles of the [[transfer function]] that are located in the right half-plane.

### [[Nyquist Plot]]

The [[Nyquist plot]] is a graphical representation of the frequency response of a system. It consists of plotting the real part of the [[transfer function]] against its imaginary part as frequency varies from 0 to infinity.

## Example

Consider a system with the [[transfer function]]:

$$ G(s) = \frac{K}{s(s+1)} $$

To determine the stability of this system using the Nyquist criterion, we first need to find its [[Nyquist plot]]. By evaluating $G(j\omega)$ for $\omega$ ranging from 0 to infinity, we can plot points on the complex plane.

Next, we analyze how many times the plot encircles (-1,0) in a counterclockwise direction. If it encircles it exactly once, then there is one pole in the right half-plane and thus one unstable mode. If it does not encircle (-1,0) at all, then there are no unstable modes.

By applying these steps and understanding how to interpret Nyquist plots correctly, we can effectively use the Nyquist criterion to assess stability in control systems.