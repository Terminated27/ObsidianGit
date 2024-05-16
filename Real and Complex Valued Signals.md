#math #Conttime 

In signal processing, signals can be classified into two types based on the values they take: **real valued signals** and **complex valued signals**. 

## Real Valued Signals

A [[real valued signal]] is a signal whose values are real numbers. Mathematically, a [[real valued signal]] can be represented as $x(t)$, where $t$ is the independent variable (usually time) and $x(t)$ is the value of the signal at time $t$. The domain of a [[real valued signal]] can be continuous or discrete.

### Example 1: Continuous [[Real Valued Signal]]

Consider a continuous [[real valued signal]] given by:

$$
x(t) = \sin(2\pi f t)
$$

where $f$ is the frequency of the sinusoidal waveform. This represents a sine wave with frequency $f$.

### Example 2: Discrete [[Real Valued Signal]]

Consider a discrete [[real valued signal]] given by:

$$
x[n] = \cos(\omega n)
$$

where $\omega$ is the angular frequency and $n$ is an integer representing discrete time instances. This represents a cosine wave with angular frequency $\omega$.

## Complex Valued Signals

A complex valued signal is a signal whose values are complex numbers. Mathematically, a complex valued signal can be represented as $z(t)$, where $t$ is the independent variable (usually time) and $z(t)$ is the value of the signal at time $t$. Similar to real valued signals, complex valued signals can have continuous or discrete domains.

### Example 3: Continuous Complex Valued Signal

Consider a continuous complex valued signal given by:

$$
z(t) = e^{j\omega t}
$$

where $\omega$ is the angular frequency and $j=\sqrt{-1}$ represents the imaginary unit. This represents a complex exponential signal with angular frequency $\omega$.

### Example 4: Discrete Complex Valued Signal

Consider a discrete complex valued signal given by:

$$
z[n] = e^{j\omega n}
$$

where $\omega$ is the angular frequency and $n$ is an integer representing discrete time instances. This represents a complex exponential signal with angular frequency $\omega$.

## Properties of Real and Complex Valued Signals

Real valued signals have some important properties that are not applicable to complex valued signals:

1. **Symmetry**: Real valued signals can exhibit symmetry, such as even symmetry ($x(t) = x(-t)$) or odd symmetry ($x(t) = -x(-t)$). Complex valued signals do not possess such symmetry.

2. **Conjugate Symmetry**: A [[real valued signal]] can be conjugate symmetric, which means $x(t) = x^*(-t)$, where $x^*$ denotes the [[complex conjugate]] of $x$. Complex valued signals may or may not exhibit conjugate symmetry.

3. **[[Power]] Spectrum**: The [[power]] spectrum of a [[real valued signal]] is always symmetric about zero frequency. This property is not applicable to complex valued signals.

## Conclusion

Real and complex valued signals are fundamental concepts in signal processing. Real valued signals have values that are real numbers, while complex valued signals have values that are complex numbers. Understanding the properties and characteristics of these two types of signals is crucial for analyzing and processing various types of data.