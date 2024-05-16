#Conttime 

In signal processing, the [[power]] of a time signal is a crucial concept that helps in understanding the [[energy]] distribution of the signal over time. The [[power]] of a continuous-time signal x(t) is defined as:

$$ P_x = \lim_{T \to \infty} \frac{1}{2T} \int_{-T}^{T} |x(t)|^2 dt $$

where $P_x$ represents the [[power]] of the signal x(t).

## Key Theorems and Definitions:

1. **Parseval's Theorem**: For a [[periodic signal]] x(t) with period T, the total [[power]] can be calculated using the Fourier series coefficients as:

$$ P_x = \frac{1}{T} \int_{0}^{T} |x(t)|^2 dt 
$$

where $c_n$ are the Fourier series coefficients.

2. **Energy Signal vs [[Power]] Signal**: A signal is said to be an energy signal if its total [[energy]] is finite, i.e., $\int_{-\infty}^{\infty} |x(t)|^2 dt < \infty$. On the other hand, a signal is considered a [[power]] signal if its total [[power]] is finite, i.e., $\lim_{T \to \infty} \frac{1}{2T} \int_{-T}^{T} |x(t)|^2 dt < \infty$.

## Step-by-Step Example:

Consider a simple sinusoidal signal given by:

$$ x(t) = A\cos(\omega t) $$

where A is the amplitude and $\omega$ is the angular frequency.

To calculate the [[power]] of this signal over one period (0 to $2\pi/\omega$), we use the definition of [[power]] for periodic signals:

$$ P_x = \frac{1}{T} \int_{0}^{T} |x(t)|^2 dt $$

Substitute x(t) into the equation and integrate over one period:

$$ P_x = \frac{1}{2\pi/\omega}\int_{0}^{2\pi/\omega}|A\cos(\omega t)|^2dt $$

Solving this [[integral]] gives us:

$$ P_x = \frac{A^2}{4\pi/\omega}\left[\frac{\sin(2\pi/\omega)}{4}\right] $$

Therefore, for this sinusoidal signal, the [[power]] can be calculated using this expression.

By understanding and calculating the [[power]] of time signals, we gain insights into their [[energy]] distribution and characteristics over time. This knowledge is essential in various applications such as communication systems, control systems, and image processing.