In control systems, stability refers to the behavior of a system when subjected to various inputs. Stability in the [[Laplace domain]], also known as the S domain, is crucial for analyzing and designing control systems. A system is said to be stable in the S domain if all poles of its [[transfer function]] have negative real parts.

## Key Theorems and Definitions

1. **[[Routh-Hurwitz Criterion]]**: The [[Routh-Hurwitz criterion]] is a necessary and sufficient condition for the stability of a system in the S domain. It states that all coefficients of the [[characteristic equation]] must be positive for the system to be stable.

2. **[[Nyquist Criterion]]**: The [[Nyquist criterion]] is another method used to determine stability in the S domain. It involves plotting the Nyquist diagram of the system and analyzing its encirclements around the critical point (-1, j0).

3. **[[BIBO Stability]]**: BIBO (Bounded Input Bounded Output) stability refers to a system's ability to produce bounded output for bounded input signals. A system is said to be BIBO stable if its output remains bounded for any bounded input signal.

## Step-by-Step Example

Consider a [[transfer function]] in the form of:

$$G(s) = \frac{K}{s(s+1)(s+2)}$$

To determine the stability of this system, we need to analyze its poles. The poles are located at s=0, s=-1, and s=-2. Since all poles have negative real parts, this system is stable in the S domain.

By applying the [[Routh-Hurwitz criterion]] or [[Nyquist Criterion]], we can further confirm the stability of this system.

In conclusion, understanding stability in the S domain is essential for ensuring robust and reliable control systems. By analyzing pole locations and applying stability criteria, engineers can design systems that exhibit desirable performance characteristics.