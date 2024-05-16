#math 

The fundamental period is a concept used in the field of signal processing and Fourier analysis to describe the periodicity of a function. It represents the smallest positive value of T for which a periodic function f(t) satisfies the equation:

$$
f(t + T) = f(t)
$$

In other words, if a function repeats itself after every T units of time, then T is called the fundamental period of that function.

## Theorem: Existence of Fundamental Period

Every periodic function with a well-defined period has at least one fundamental period.

## Theorem: Uniqueness of Fundamental Period

If a periodic function has a fundamental period, it is unique.

## Definition: Harmonic Function

A harmonic function is a periodic function with fundamental period T that satisfies the equation:

$$
f(t + T) = f(t)
$$

where T is the fundamental period.

## Example: Finding Fundamental Period

Consider the following periodic function:

$$
f(t) = \sin(2\pi t) + \cos(4\pi t)
$$

To find its fundamental period, we need to determine the smallest positive value of T for which f(t + T) = f(t).

Let's start by evaluating f(t + T):

$$
f(t + T) = \sin(2\pi (t+T)) + \cos(4\pi (t+T))
          = \sin(2\pi t + 2\pi T) + \cos(4\pi t + 4\pi T)
          = \sin(2\pi t)\cos(2\pi T) + \cos(2\pi t)\sin(2\pi T) \\
          - \sin(4\pi t)\sin(4\pi T) - \cos(4\pi t)\cos(4\pi T)
$$

Now, let's compare f(t + T) with f(t):

$$
f(t + T) = f(t) \\
\Rightarrow \sin(2\pi t)\cos(2\pi T) + \cos(2\pi t)\sin(2\pi T) \\
- \sin(4\pi t)\sin(4\pi T) - \cos(4\pi t)\cos(4\pi T) \\
= \sin(2\pi t) + \cos(4\pi t)
$$

From this equation, we can conclude that:

$$
\cos(2\pi T) = 1 \\
\sin(2\pi T) = 0 \\
-\sin(4\pi T) = 0 \\
-\cos(4\pi T) = 0
$$

Solving these equations, we find that:

$$
T = \frac{1}{2}
$$

Therefore, the fundamental period of the function f(t) is $\frac{1}{2}$.

## Conclusion

The fundamental period of a periodic function represents the smallest positive value of T for which the function repeats itself. It is a unique value that characterizes the periodicity of the function. By understanding and identifying the fundamental period, we can analyze and manipulate periodic functions more effectively in signal processing and Fourier analysis.