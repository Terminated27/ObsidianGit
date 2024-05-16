

# Step Response y(t)

The step response $y(t)$ of a continuous time system is defined as the output of the system when the input is a unit [[step function]] $u(t)$, which is defined as:

$$
u(t) = \begin{cases} 
0 & \text{for } t < 0 \\
1 & \text{for } t \geq 0
\end{cases}
$$

The step response $y(t)$ can be obtained by convolving the impulse response $h(t)$ of the system with the unit [[step function]] $u(t)$:

$$
y(t) = h(t) * u(t) = \int_{-\infty}^{\infty} h(\tau)u(t-\tau)d\tau
$$

The [[Laplace transform]] of the step response $Y(s)$ can be related to the [[Laplace transform]] of the impulse response $H(s)$ by:

$$
Y(s) = H(s)U(s)
$$

where $U(s)$ is the [[Laplace transform]] of the unit [[step function]].

The key theorem related to step response is that if a system has a bounded input bounded output (BIBO) stable impulse response, then its step response will also be BIBO stable.

### Example

Consider a system with impulse response given by:

$$
h(t) = e^{-at}u(t)
$$

where $a > 0$. The step response can be calculated as:

$$
\begin{aligned}
y(t) &= h(t)*u(t) \\
&= \int_{0}^{t} e^{-a\tau}d\tau \\
&= -\frac{1}{a}(e^{-at}-1)
\end{aligned}
$$

Thus, for this system, the step response is given by $y(t) = -\frac{1}{a}(e^{-at}-1)$ for $t \geq 0$.