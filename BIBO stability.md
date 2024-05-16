#Conttime 

BIBO (Bounded Input, Bounded Output) stability is a key concept in control theory that deals with the behavior of a system when subjected to bounded input signals. A system is said to be BIBO stable if, for any bounded input signal, the output remains bounded as well.

## Definition
A system described by the [[transfer function]] $G(s)$ is said to be BIBO stable if for every bounded input signal $x(t)$ with $\lVert x(t) \rVert < M$, the output $y(t)$ satisfies $\lVert y(t) \rVert < N$ for some constant $N$.

## Key Theorem
The BIBO stability of a system can be determined by analyzing the poles of its [[transfer function]]. A system is BIBO stable if and only if all the poles of its [[transfer function]] lie in the left half of the complex plane.

Denominator degree is larger or equal to the degree of the numerator

If [[transfer function]] is improper and rational, will never be BIBO stable
## Example
Consider a system with [[transfer function]] $G(s) = \frac{1}{s+1}$. To determine its BIBO stability, we need to analyze the pole at $s=-1$. Since this pole lies in the left half of the complex plane, the system is BIBO stable.

By considering the poles of a [[transfer function]], we can quickly assess whether a system is BIBO stable without explicitly solving for its output response. This property simplifies stability analysis and design in control systems.