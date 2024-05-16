

# LTI Time Invariance

In the context of Linear Time-Invariant (LTI) systems, time invariance refers to a property where the system's response to a shifted input signal is also shifted by the same amount. Mathematically, a system is said to be time-invariant if for any input signal $x(t)$ and corresponding output signal $y(t)$, the following condition holds:

$$
y(t - \tau) = T[x(t - \tau)]
$$

where $\tau$ is a time shift and $T[\cdot]$ represents the system operation.

## Key Theorems and Definitions

1. **Time Invariance Property**: A system is said to be time-invariant if its output response to a delayed input signal is simply a delayed version of the output response to the original input signal.

2. **Impulse Response**: The impulse response of an LTI system is defined as the output of the system when an impulse function $\delta(t)$ is applied as input. It characterizes how the system responds to sudden changes in input.

3. **[[Convolution]]**: The output of an LTI system can be obtained by convolving the input signal with the impulse response of the system. Mathematically, this can be expressed as:

$$
y(t) = x(t) * h(t)
$$

where $*$ denotes [[convolution]] and $h(t)$ is the impulse response.

## Step-by-Step Example

Consider an LTI system with impulse response $h(t) = e^{-t}u(t)$, where $u(t)$ is the unit [[step function]]. If we apply an input signal $x(t) = e^{2t}u(t)$ to this system, we can find the output using [[convolution]]:

$$
y(t) = x(t) * h(t) = \int_{-\infty}^{\infty} x(\tau)h(t-\tau)d\tau
$$

Substitute $x(\tau)$ and $h(t-\tau)$ into the [[integral]]:

$$
y(t) = \int_{0}^{t} e^{2\tau}e^{-(t-\tau)}d\tau \\
= \int_{0}^{t} e^{\tau + t - \tau}d\tau \\
= \int_{0}^{t} e^td\tau \\
= te^t
$$

Therefore, the output response of this LTI system to the given input signal is $y(t) = te^t$, which satisfies the time invariance property.

By understanding and applying these key concepts related to LTI time invariance, we can analyze and predict how linear systems respond to different inputs over time shifts accurately.