#Conttime 

In the field of signal processing, various operations are performed on signals to manipulate and analyze their properties. These operations help in understanding and extracting useful information from signals. In this atomic note, we will discuss some key operations on signals, including signal addition, multiplication, [[convolution]], and [[Fourier transform]].

## Signal Addition
Signal addition is a basic operation that combines two signals into a single signal. Let's consider two continuous-time signals $x(t)$ and $y(t)$:

$$
x(t) = A \cos(\omega_1 t + \phi_1)
$$

$$
y(t) = B \cos(\omega_2 t + \phi_2)
$$

where $A$, $B$, $\omega_1$, $\omega_2$, $\phi_1$, and $\phi_2$ are constants representing the amplitudes, frequencies, and phases of the signals.

The sum of these two signals is given by:

$$
z(t) = x(t) + y(t)
$$

To compute the sum, we simply add the corresponding terms:

$$
z(t) = A \cos(\omega_1 t + \phi_1) + B \cos(\omega_2 t + \phi_2)
$$

## Signal Multiplication
Signal multiplication is another important operation that combines two signals into a single signal. Let's consider the same two continuous-time signals $x(t)$ and $y(t)$ as before.

The product of these two signals is given by:

$$
z(t) = x(t) \cdot y(t)
$$

To compute the product, we multiply the corresponding terms:

$$
z(t) = A \cos(\omega_1 t + \phi_1) \cdot B \cos(\omega_2 t + \phi_2)
$$

## [[Convolution]]
[[Convolution]] is a fundamental operation in signal processing that combines two signals to produce a third signal. It is often used to model the output of a linear time-invariant (LTI) system when the input is known.

Let's consider two discrete-time signals $x[n]$ and $h[n]$. The [[convolution]] of these two signals is given by:

$$
y[n] = x[n] * h[n] = \sum_{k=-\infty}^{\infty} x[k] \cdot h[n-k]
$$

where $*$ denotes the [[convolution]] operator.

[[Convolution]] can be thought of as a sliding dot product between the two signals, where one signal is flipped and shifted over the other signal. The resulting signal represents the combined effect of both signals.

## [[Fourier Transform]]
The [[Fourier transform]] is a powerful tool for analyzing signals in the frequency domain. It decomposes a signal into its constituent frequencies, revealing the frequency content of the signal.

The [[Fourier transform]] of a continuous-time signal $x(t)$ is given by:

$$
X(\omega) = \int_{-\infty}^{\infty} x(t) e^{-j\omega t} dt
$$

where $X(\omega)$ represents the frequency spectrum of the signal.

Similarly, the [[Fourier transform]] of a discrete-time signal $x[n]$ is given by:

$$
X(e^{j\omega}) = \sum_{n=-\infty}^{\infty} x[n] e^{-j\omega n}
$$

The inverse [[Fourier transform]] can be used to reconstruct the original signal from its frequency spectrum.

These operations on signals play a crucial role in various applications such as audio processing, image processing, communications, and control systems. Understanding these operations and their properties helps in designing efficient [[algorithms]] and systems for manipulating and analyzing signals.