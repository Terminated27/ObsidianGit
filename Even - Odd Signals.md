#Conttime 

In signal processing, a **signal** is a function that conveys information about a phenomenon. Signals can be classified into different categories based on their properties. One such classification is based on whether the signal is **even** or **odd**.

## Definitions

A signal $x(t)$ defined over the entire real line is said to be **even** if it satisfies the condition:

$$x(t) = x(-t) \quad \forall t$$

Similarly, a signal $x(t)$ is said to be **odd** if it satisfies:

$$x(t) = -x(-t) \quad \forall t$$

In other words, an even signal is symmetric about the y-axis, while an odd signal is anti-symmetric about the y-axis.
upside down A = for all or for any
## Properties of Even and Odd Signals

1. If $x(t)$ is even, then its [[Fourier transform]] $X(f)$ is also even.
2. If $x(t)$ is odd, then its [[Fourier transform]] $X(f)$ is purely imaginary and odd.
3. Any signal can be expressed as a sum of an even and an odd part:

   $$x(t) = x_e(t) + x_o(t)$$
   
   where $x_e(t)$ represents the even part of the signal and $x_o(t)$ represents the odd part of the signal.
   
4. The product of two even signals or two odd signals results in an even signal.
5. The product of an even and an odd signal results in an odd signal.

## Examples

### Example 1: Determining Evenness/Oddness using Symmetry

Consider a continuous-time signal defined by:

$$
x_1(t) = 
\begin{cases}
2 & \text{if } -3 \leq t < 0 \\
-2 & \text{if } 0 \leq t < 3 \\
\end{cases}
$$

To determine if $x_1(t)$ is even or odd, we can check its symmetry.

**Step 1:** Check for even symmetry:

$$x_1(t) = x_1(-t) \quad \forall t$$

Substituting $-t$ for $t$ in the given signal:

$$
x_1(-t) = 
\begin{cases}
2 & \text{if } 3 \leq t < 0 \\
-2 & \text{if } 0 \leq t < -3 \\
\end{cases}
$$

Since $x_1(t)$ is not equal to $x_1(-t)$ for all values of $t$, it is not an even signal.

**Step 2:** Check for odd symmetry:

$$x_1(t) = -x_1(-t) \quad \forall t$$

Substituting $-t$ for $t$ in the given signal:

$$
-x_1(-t) = 
\begin{cases}
-2 & \text{if } 3 \leq t < 0 \\
2 & \text{if } 0 \leq t < -3 \\
\end{cases}
$$

Since $x_1(t)$ is equal to $-x_1(-t)$ for all values of $t$, it is an odd signal.
