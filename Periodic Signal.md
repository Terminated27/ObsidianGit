#math #Conttime 

A periodic signal is a signal that repeats itself after a certain period of time. It is characterized by its fundamental frequency, which is the reciprocal of the period. In this atomic note, we will explore the properties and mathematical representation of periodic signals.

## Definitions

**Period**: The period $T$ of a periodic signal is the smallest positive value for which the signal repeats itself. Mathematically, a signal $x(t)$ is periodic with period $T$ if $x(t) = x(t + T)$ for all $t$.

**Frequency**: The frequency $f$ of a periodic signal is defined as the reciprocal of the period, i.e., $f = \frac{1}{T}$. It represents the number of cycles per unit time.

**Amplitude**: The amplitude $A$ of a periodic signal represents its maximum magnitude. It indicates the range within which the signal varies.

## Mathematical Representation

A periodic signal can be mathematically represented using Fourier series. Fourier series allows us to express any periodic function as an infinite sum of sinusoidal functions (sines and cosines) or complex exponentials.

The general form of a Fourier series representation for a periodic signal $x(t)$ with period $T$ is given by:

$$
x(t) = \sum_{n=-\infty}^{\infty} c_n e^{j\frac{2\pi n}{T} t}
$$

where $c_n$ are called the Fourier coefficients and are given by:

$$
c_n = \frac{1}{T} \int_{-\frac{T}{2}}^{\frac{T}{2}} x(t) e^{-j\frac{2\pi n}{T} t} dt
$$

The Fourier coefficients determine the contribution of each harmonic component to the overall shape of the periodic signal.

## Properties

Periodic signals exhibit several important properties:

**Linearity**: If $x_1(t)$ and $x_2(t)$ are periodic signals with periods $T_1$ and $T_2$ respectively, and $a$ and $b$ are constants, then the signal $ax_1(t) + bx_2(t)$ is also periodic with period $\text{lcm}(T_1, T_2)$ (least common multiple of $T_1$ and $T_2$).

**Time Shifting**: If $x(t)$ is a periodic signal with period $T$, then the signal $x(t - t_0)$ is also periodic with period $T$. This means that shifting a periodic signal in time does not change its fundamental frequency.

**Time Scaling**: If $x(t)$ is a periodic signal with period $T$, then the signal $x(at)$ is also periodic with period $\frac{T}{|a|}$. This means that scaling a periodic signal in time changes its fundamental frequency.

**Frequency Shifting**: If $x(t)$ is a periodic signal with fundamental frequency $\omega$, then the signal $\cos(\omega t + \phi)$ or $\sin(\omega t + \phi)$ is also a periodic signal with the same fundamental frequency. The [[phase]] shift $\phi$ only affects the initial [[phase]] of the sinusoidal component.

## Example

Consider a square wave defined as:

$$
x(t) = \begin{cases} 
      1 & 0 < t < T/2 \\
      -1 & T/2 < t < T
   \end{cases}
$$

where $T$ is the period of the square wave. We can find its Fourier series representation by calculating the Fourier coefficients:

$$
c_n = \frac{1}{T} \int_{-\frac{T}{2}}^{\frac{T}{2}} x(t) e^{-j\frac{2\pi n}{T} t} dt
$$

For $n = 0$, the [[integral]] becomes:

$$
c_0 = \frac{1}{T} \int_{-\frac{T}{2}}^{\frac{T}{2}} x(t) dt = \frac{1}{T} \left(\int_{0}^{\frac{T}{2}} 1 dt + \int_{\frac{T}{2}}^{T} -1 dt\right) = 0
$$

For $n \neq 0$, the [[integral]] becomes:

$$
c_n = \frac{1}{T} \left(\int_{0}^{\frac{T}{2}} e^{-j\frac{2\pi n}{T} t} dt - \int_{\frac{T}{2}}^{T} e^{-j\frac{2\pi n}{T} t} dt\right)
$$

Solving these integrals, we find:

$$
c_n = \begin{cases}
      0 & n \text{ is even}\\
      -j\frac{2}{n\pi} & n \text{ is odd}
   \end{cases}
$$

Substituting these coefficients in the Fourier series representation, we obtain:

$$
x(t) = -j\sum_{n=-\infty, n~odd}^{\infty}\left(\frac{2}{n\pi}\right)e^{j\omega_n t}
$$

where $\omega_n = \frac{2n\pi}{T}$.

This example demonstrates how Fourier series can be used to represent periodic signals and provides insight into the harmonic components present in a square wave.

## Conclusion

Periodic signals are fundamental in understanding the behavior of many real-world phenomena. Fourier series provides a powerful tool for analyzing and representing periodic signals in terms of their harmonic components. Understanding the properties and mathematical representation of periodic signals is essential in various fields, including signal processing, communications, and control systems.