

In the field of signal processing and control systems, linear time-invariant (LTI) systems play a crucial role. These systems have several important properties that make their analysis and design relatively straightforward. In this atomic note, we will explore the key concepts, theorems, and definitions related to LTI systems.
[[LTI Linearity]]
[[LTI Time Invariance]]

## Definition

An LTI system is a mathematical model used to describe the input-output relationship of a system that is both linear and time-invariant. 

**Linearity** means that if the input to the system is a linear combination of signals $x_1(t)$ and $x_2(t)$, then the output of the system will be a linear combination of their respective outputs $y_1(t)$ and $y_2(t)$. Mathematically, this can be expressed as:

$$
\begin{align*}
\text{If } y_1(t) &= \mathcal{L}\{x_1(t)\} \text{ and } y_2(t) = \mathcal{L}\{x_2(t)\}, \\
\text{then } \mathcal{L}\{\alpha x_1(t) + \beta x_2(t)\} &= \alpha y_1(t) + \beta y_2(t),
\end{align*}
$$

where $\alpha$ and $\beta$ are arbitrary constants.

**Time-invariance** means that if an input signal $x(t)$ produces an output signal $y(t)$, then any time-shifted version of the input signal $\tilde{x}(t) = x(t - t_0)$ will produce a time-shifted version of the output signal $\tilde{y}(t) = y(t - t_0)$ for any constant time shift $t_0$. Mathematically, this can be expressed as:

$$
\begin{align*}
\text{If } y(t) &= \mathcal{L}\{x(t)\}, \\
\text{then } \mathcal{L}\{\tilde{x}(t)\} &= \tilde{y}(t),
\end{align*}
$$

where $\tilde{x}(t)$ and $\tilde{y}(t)$ represent the time-shifted input and output signals, respectively.

## Impulse Response

The impulse response of an LTI system is a fundamental concept used to characterize these systems. It represents the output of the system when the input is an impulse function $\delta(t)$, also known as the [[Dirac delta function]]. Mathematically, this can be expressed as:

$$
h(t) = \mathcal{L}\{\delta(t)\},
$$

where $h(t)$ is the impulse response of the system.

The impulse response provides a complete description of an LTI system since any input signal $x(t)$ can be represented as a weighted sum of shifted and scaled impulse functions:

$$
x(t) = \int_{-\infty}^{\infty} x(\tau) \delta(t - \tau) d\tau.
$$

By exploiting the linearity and time-invariance properties, we can compute the output $y(t)$ for any input signal $x(t)$ using [[convolution]]:

$$
y(t) = x(t) * h(t),
$$

where $*$ denotes [[convolution]].

## [[Transfer Function]]

The [[transfer function]] is another important concept in LTI systems. It provides a frequency-domain representation of the system's behavior. The [[transfer function]] $H(\omega)$ is defined as the [[Fourier transform]] of the impulse response $h(t)$:

$$
H(\omega) = \int_{-\infty}^{\infty} h(t) e^{-j\omega t} dt.
$$

The [[transfer function]] can also be expressed in terms of the [[Laplace transform]]. If the impulse response is denoted as $h(t)$, then the [[transfer function]] $H(s)$ is given by:

$$
H(s) = \mathcal{L}\{h(t)\}.
$$

The [[transfer function]] allows us to analyze the system's response to different frequency components of an input signal. By evaluating $H(\omega)$ at different frequencies, we can determine how the system amplifies or attenuates each frequency component.

## Stability

Stability is a crucial property of LTI systems. A system is considered stable if its output remains bounded for any bounded input signal. There are two types of stability: **bounded-input bounded-output (BIBO) stability** and **internal stability**.

A system is BIBO stable if, for any bounded input signal $x(t)$, the corresponding output signal $y(t)$ remains bounded. Mathematically, this can be expressed as:

$$
\int_{-\infty}^{\infty} |x(t)| dt < \infty \implies \int_{-\infty}^{\infty} |y(t)| dt < \infty.
$$

Internal stability refers to the behavior of the system when it is not driven by an external input. An LTI system is internally stable if its impulse response $h(t)$ decays as $t$ approaches infinity.

## Conclusion

Linear time-invariant (LTI) systems are widely used in signal processing and control applications due to their well-defined properties and ease of analysis. In this atomic note, we discussed the definition of LTI systems, their linearity and time-invariance properties, impulse response representation, [[convolution]] operation, [[transfer function]] representation, and stability concepts. These fundamental concepts provide a solid foundation for the analysis and design of LTI systems.