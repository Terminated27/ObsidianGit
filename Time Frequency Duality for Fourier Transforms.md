
In the realm of signal processing, the concept of time-frequency duality plays a crucial role in understanding the behavior of signals in both time and frequency domains. When we consider continuous time signals and their Fourier transforms, this duality becomes particularly significant.

## Definition

The [[Fourier transform]] of a continuous time signal $x(t)$ is defined as:

$$X(\omega) = \int_{-\infty}^{\infty} x(t)e^{-j\omega t} dt$$

where $X(\omega)$ represents the frequency domain representation of the signal.

## Theorem: Time-Frequency Duality

The time-frequency duality theorem states that there is an inherent trade-off between how localized a signal is in the time domain and how spread out it is in the frequency domain. Mathematically, this can be expressed as:

$$\Delta t \cdot \Delta \omega \geq \frac{1}{2}$$

where $\Delta t$ is the temporal spread of the signal in time domain and $\Delta \omega$ is its spread in frequency domain.

## Example: Gaussian Signal

Consider a Gaussian signal given by:

$$x(t) = e^{-\alpha t^2}$$

where $\alpha > 0$. The [[Fourier transform]] of this signal can be calculated as:

$$X(\omega) = \sqrt{\frac{\pi}{\alpha}} e^{-\frac{\omega^2}{4\alpha}}$$

This example illustrates how a signal that is highly localized in the time domain (due to exponential decay) results in a broader spread in the frequency domain.

By exploring such examples and understanding the implications of time-frequency duality, we gain deeper insights into the behavior of continuous time signals and their corresponding Fourier transforms.