#Conttime 

The impulse response of a continuous-time system is defined as the output of the system when the input is an impulse function $\delta(t)$, denoted as $h(t)$. It characterizes the behavior of a system in response to an instantaneous input.

## Properties of Impulse Response

1. **Linearity**: If a system is linear, the impulse response satisfies the [[superposition]] principle:
$$
h(a_1t_1 + a_2t_2) = a_1h(t_1) + a_2h(t_2)
$$

2. **Time Invariance**: For time-invariant systems, the impulse response remains constant over time:
$$
h(t - t_0) = h(t)
$$

3. **Causality**: A causal system has an impulse response that is zero for negative times:
$$
h(t) = 0 \text{ for } t < 0
$$

## [[Convolution]] [[Integral]]

The output $y(t)$ of a continuous-time LTI system with impulse response $h(t)$ and input signal $x(t)$ can be expressed as the [[convolution]] [[integral]]:
$$
y(t) = x(t) * h(t) = \int_{-\infty}^{\infty} x(\tau)h(t - \tau)d\tau
$$

## Example: Computing Output using Impulse Response

Consider an LTI system with impulse response $h(t) = e^{-t}u(t)$, where $u(t)$ is the unit [[step function]]. If the input signal is $x(t) = u(t)$, then the output can be computed as:
$$
y(t) = x(t) * h (t)= \int_{0}^{t} e^{-\tau}d\tau = 1 - e^{-t}
$$

By understanding the impulse response of a continuous-time system, we can analyze and predict its behavior for various input signals.