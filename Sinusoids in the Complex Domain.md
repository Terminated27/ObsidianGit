

# Sinusoids in the Complex Domain

In the complex domain, sinusoids can be represented using complex exponential functions. A sinusoid of frequency $\omega$ and amplitude $A$ can be written as:

$$x(t) = A\cdot e^{j\omega t}$$

where $j$ is the imaginary unit.

## [[Euler's Formula]]

[[Euler's formula]] relates complex exponentials to trigonometric functions:

$$e^{j\theta} = \cos(\theta) + j\sin(\theta)$$

This formula is fundamental in understanding the relationship between sinusoids and complex exponentials.

## Phasors

Phasors are complex numbers that represent sinusoidal signals. They simplify the analysis of sinusoids in the frequency domain. The phasor representation of a sinusoid $x(t) = A\cdot \cos(\omega t + \phi)$ is:

$$X(j\omega) = A\cdot e^{j\phi}$$

## [[Fourier Transform]] of Sinusoids

The [[Fourier transform]] of a sinusoid $x(t) = A\cdot \cos(\omega t)$ is given by:

$$X(j\Omega) = \pi(A/2)(\delta(\Omega - \omega) + \delta(\Omega + \omega))$$

where $\delta$ represents the [[Dirac delta function]].

## Example: [[Fourier Transform]] of a Sinusoid

Let's find the [[Fourier transform]] of $x(t) = 2\cdot \cos(3t)$ using [[Euler's formula]]:

Using [[Euler's formula]], we can rewrite $x(t)$ as:

$$x(t) = 2\cdot \cos(3t) = e^{j3t} + e^{-j3t}$$

Taking the [[Fourier transform]], we get:

$$X(j\Omega) = \pi(1/2)(2\pi[\delta(\Omega - 3) + \delta(\Omega + 3)])$$

Thus, the [[Fourier transform]] of $x(t)$ is $X(j\Omega) = 2\pi[\delta(\Omega - 3) + \delta(\Omega + 3)]$.