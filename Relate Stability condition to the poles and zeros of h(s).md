
In control systems, the stability of a system is closely related to the poles and zeros of its [[transfer function]]. The stability of a system can be determined by analyzing the locations of the poles and zeros in the complex plane.

### Key Theorems and Definitions

1. **[[Routh-Hurwitz Criterion]]**: This criterion states that for a system to be stable, all the coefficients of the [[characteristic equation]] must be positive.
   
2. **[[Nyquist Criterion]]**: This criterion states that if the [[Nyquist plot]] encircles the critical point (-1, j0) in a counterclockwise direction, then the system is unstable.

### Relating Stability Condition to Poles and Zeros

The stability of a system can be determined by examining the locations of its poles and zeros in the complex plane. 

- If all poles have negative real parts, then the system is stable.
- If any pole has a positive real part, then the system is unstable.
- If there are poles on the imaginary axis or with zero real parts, further analysis is needed using Nyquist or other stability criteria.
* same amount of poles as zeros
The [[transfer function]] $H(s)$ can be written as:

$$
H(s) = \frac{N(s)}{D(s)}
$$

Where $N(s)$ represents the numerator polynomial and $D(s)$ represents the denominator polynomial.

The poles of $H(s)$ are given by setting $D(s) = 0$:

$$
D(s) = 0
$$

Solving this equation gives us the locations of the poles in terms of $s$. Similarly, setting $N(s) = 0$ gives us the locations of zeros.

By analyzing these pole-zero plots in relation to stability criteria such as Routh-Hurwitz or Nyquist, we can determine whether a system is stable or not based on its [[transfer function]].

### Step-by-Step Example

Consider a [[transfer function]]:

$$
H(s) = \frac{s + 1}{s^2 + s + 1}
$$

The denominator polynomial has roots at:

$$
s^2 + s + 1 = 0
$$

Solving this quadratic equation gives us two [[complex conjugate]] poles with negative real parts. Therefore, based on pole-zero analysis, we can conclude that this system is stable.

By relating stability conditions to pole-zero analysis, we can gain insights into how different configurations of poles and zeros affect system stability.