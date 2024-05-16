
The **Fourier Transform** is a mathematical technique that transforms a function of time, a signal, into a function of frequency. This is particularly useful for continuous time signals.

## Definition

The Fourier Transform of a continuous time signal $x(t)x(t)$ is given by:

$$X(f) = \int_{-\infty}^{\infty} x(t) e^{-j2\pi ft} dt$$

where:

- $X(f)$ is the Fourier Transform of $x(t)$ff is the frequency variable
- $j$ is the imaginary unit

The [[Inverse Fourier Transform]] is given by:

$$x(t) = \frac{1}{2\pi}\int_{-\infty}^{\infty} X(\omega)e^{j\omega t} d\omega$$

## Properties
![[Pasted image 20240428180935.png]]
Here are some key properties of the Fourier Transform:

1. **Linearity**: The Fourier Transform of a linear combination of signals is the linear combination of their Fourier Transforms.

$$\mathcal{F}\{a x_1(t) + b x_2(t)\} = a X_1(f) + b X_2(f)$$

2. **Time Shifting**: Shifting a signal in time shifts the [[phase]] of its Fourier Transform.

$$\mathcal{F}\{x(t-t_0)\} = e^{-j2\pi f t_0} X(f)$$

3. **Frequency Shifting**: Shifting the Fourier Transform of a signal in frequency shifts the signal in time.

$$\mathcal{F}^{-1}\{X(f-f_0)\} = e^{j2\pi t f_0} x(t)$$

## Example

Let’s consider a simple example of a continuous time signal, a rectangular pulse x(t)x(t) of width TT:

```markdown
x(t) = {1 for |t| < T/2, 0 otherwise}
```

The Fourier Transform of this signal is given by:
$$
\begin{align}
X(f) &= \int_{-T/2}^{T/2} e^{-j2πft} dt\\
     &= [ -1/(j2πf) e^{-j2πft} ]_{-T/2}^{T/2}\\
     &= T sinc(fT)
\end{align}
$$

where $sinc(x) = sin(πx)/(πx)$

This shows that the Fourier Transform of a time-limited signal is not band-limited (it exists for all frequencies), demonstrating a key principle in signal processing.

I hope this note provides a deeper understanding of the Fourier Transform for continuous time signals!