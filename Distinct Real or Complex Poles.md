#Conttime 
In control systems, poles play a crucial role in determining the stability and dynamic response of the system. Poles can be real or complex, and when they are distinct (i.e., not repeated), they provide valuable insights into the system's behavior.

## Definition
A pole of a [[transfer function]] is a value of s for which the denominator of the [[transfer function]] becomes zero. When these poles are distinct, they are unique and do not repeat.

## Theorem
For a linear time-invariant system described by a [[transfer function]] $G(s)$, if the poles are distinct real numbers $p_1$ and $p_2$, then the system response can be written as:
$$
y(t) = K_1e^{p_1t} + K_2e^{p_2t}
$$

## Example
Consider a system with a [[transfer function]] $G(s) = \frac{1}{s^2 + 3s + 2}$. The poles of this system are found by setting the denominator equal to zero:
$$
s^2 + 3s + 2 = 0
$$
Solving for s, we get $s = -1$ and $s = -2$, which are distinct real poles.

Therefore, the system response can be expressed as:
$$
y(t) = K_1e^{-t} + K_2e^{-2t}
$$

## Example
Consider a system with a [[transfer function]] $G(s) = \frac{1}{(s+1)^2}$. The poles of this system are found by setting the denominator equal to zero:
$$
(s+1)^2 = 0
$$
Solving for s, we get $s = -1$, which is a repeated pole.

Therefore, the system response can be expressed as:
$$
y(t) = (K_1 + K_2t)e^{-t}
$$
where $K_1$ and $K_2$ are constants determined by the initial conditions of the system.
## Theorem
If the poles of a system are [[complex conjugate]] pairs $-a \pm jb$, where $a$ is real and $b$ is imaginary, then the system response can be written as:
$$
y(t) = e^{-at}(K_1\cos(bt) + K_2\sin(bt))
$$

## Example
Consider a system with [[complex conjugate]] poles at $-1 \pm j$. The system response can be expressed as:
$$
y(t) = e^{-t}(K_1\cos(t) + K_2\sin(t))
$$

By understanding how distinct real or complex poles affect the system's behavior, engineers can design control systems that exhibit desired stability and performance characteristics.
