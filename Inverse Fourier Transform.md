#Conttime 
# Inverse [[Fourier Transform]]

The Inverse [[Fourier Transform]] is an important mathematical operation in signal processing that allows us to convert a signal from the frequency domain to the time domain. It is the inverse of the [[Fourier Transform]], which converts a signal from the time domain to the frequency domain.

## Definition

The Inverse [[Fourier Transform]] of a continuous time signal $x(t)$ is given by:

$$x(t) = \frac{1}{2\pi}\int_{-\infty}^{\infty} X(\omega)e^{j\omega t} d\omega$$

where $X(\omega)$ is the [[Fourier Transform]] of $x(t)$.

## Key Theorems

### Parseval's Theorem

Parseval's theorem states that the energy of a signal in the time domain is equal to its energy in the frequency domain. Mathematically, it can be expressed as:

$$\int_{-\infty}^{\infty}|x(t)|^2 dt = \frac{1}{2\pi}\int_{-\infty}^{\infty}|X(\omega)|^2 d\omega$$

### [[Convolution]] Theorem

The [[Convolution]] Theorem states that [[convolution]] in one domain corresponds to multiplication in the other domain. Mathematically, it can be expressed as:

$$x(t) * h(t) \longleftrightarrow X(\omega)H(\omega)$$

where $*$ denotes [[convolution]] and $\longleftrightarrow$ denotes correspondence.

## Step-by-Step Example

Let us consider a continuous time signal $x(t)$ given by:

$$x(t) = e^{-at}u(t)$$

where $a$ is a positive constant and $u(t)$ is the unit [[step function]].

To find its Inverse [[Fourier Transform]], we first need to find its [[Fourier Transform]] using the definition:

$$X(\omega) = \int_{-\infty}^{\infty} e^{-at}u(t)e^{-j\omega t} dt$$

Applying the properties of the unit [[step function]], we get:

$$X(\omega) = \int_{0}^{\infty} e^{-(a+j\omega)t} dt = \frac{1}{a+j\omega}$$

Now, using the definition of Inverse [[Fourier Transform]], we get:

$$x(t) = \frac{1}{2\pi}\int_{-\infty}^{\infty}\frac{e^{-(a+j\omega)t}}{a+j\omega} d\omega$$

Solving this [[integral]] using complex analysis techniques, we get:

$$x(t) = \frac{1}{2a}\left(1-e^{-at}\right)u(t)$$

This is the final expression for the Inverse [[Fourier Transform]] of $x(t)$.

## Conclusion

The Inverse [[Fourier Transform]] is a powerful tool in signal processing that allows us to analyze signals in both time and frequency domains. It has many applications in fields such as communication, image and audio processing, and control systems. Understanding its properties and theorems is essential for anyone working with continuous time signals. 