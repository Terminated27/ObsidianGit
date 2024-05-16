#math #Conttime
[[Non-Causal Signal]]
A causal signal is a fundamental concept in signal processing and is often used to model real-world phenomena. In this atomic note, we will explore the definition of a causal signal, discuss key theorems related to causality, and provide step-by-step examples to illustrate its application.
![[Pasted image 20240205102419.png]]
## Definition

A signal is said to be causal if its value at any given time depends only on past or present values of the signal and not on future values. Mathematically, a discrete-time signal x[n] is causal if it satisfies the condition:

$$
x[n] = 0 \quad \text{for all } n < 0
$$

In other words, a causal signal has non-zero values only for non-negative time indices.

## Theorems

### Theorem 1: Causality in Linear Time-Invariant (LTI) Systems

If an LTI system with impulse response h[n] is stable, then the output y[n] of the system resulting from an input x[n] will be causal if and only if x[n] is causal.

### Proof:

Let's assume that x[n] is a causal input signal and y[n] is the output of the LTI system. We can express y[n] as the [[convolution]] sum:

$$
y[n] = \sum_{k=-\infty}^{\infty} x[k]h[n-k]
$$

Since x[k]=0 for k<0 (due to causality), we can rewrite the above sum as:

$$
y[n] = \sum_{k=0}^{\infty} x[k]h[n-k]
$$

This shows that y[n] depends only on past or present values of x[k], which implies that y[n] is also a causal signal.

Conversely, if an LTI system with impulse response h[n] is stable and the input x[n] is non-causal, then the output y[n] will not be causal. This can be proven by considering a counterexample.

### Theorem 2: Causality in Frequency Domain

A signal x(t) (continuous-time) or x[n] (discrete-time) is causal if and only if its [[Fourier transform]] X(f) (continuous-time) or X(e^(jω)) (discrete-time) is analytic in the upper half of the complex plane.

### Proof:

Let's assume that x(t) or x[n] is a causal signal with [[Fourier transform]] X(f) or X(e^(jω)). By the Paley-Wiener theorem, if a function is analytic in the upper half of the complex plane, its [[Fourier transform]] must vanish for negative frequencies. Therefore, if X(f) or X(e^(jω)) is zero for f<0 or ω<0, respectively, then x(t) or x[n] must be causal.

Conversely, if X(f) or X(e^(jω)) has non-zero values for f<0 or ω<0, respectively, then x(t) or x[n] cannot be causal.

## Examples

Let's consider two examples to illustrate the concept of causality:

### Example 1: Causal Signal

Consider a discrete-time signal defined as:

$$
x[n] = \begin{cases} 
      n & \text{for } n \geq 0 \\
      0 & \text{otherwise}
   \end{cases}
$$

This signal satisfies the condition for causality since it has non-zero values only for non-negative time indices.

### Example 2: [[Non-Causal Signal]]

Consider another discrete-time signal defined as:

$$
x[n] = \begin{cases} 
      n & \text{for } n \leq 0 \\
      0 & \text{otherwise}
   \end{cases}
$$

This signal violates the condition for causality since it has non-zero values for negative time indices.

## Conclusion

Causal signals play a crucial role in signal processing, and understanding their properties is essential for designing and analyzing systems. In this atomic note, we defined a causal signal, discussed key theorems related to causality in LTI systems and the frequency domain, and provided step-by-step examples to illustrate these concepts.