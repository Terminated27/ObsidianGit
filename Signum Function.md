#math 
The signum function, denoted as $\text{sgn}(x)$ or $\text{sign}(x)$, is a mathematical function that returns the sign of a real number. It is defined as follows:

$$
\text{sgn}(x) = \begin{cases} 
-1 & \text{if } x < 0 \\
0 & \text{if } x = 0 \\
1 & \text{if } x > 0 
\end{cases}
$$

The signum function can also be defined using the absolute value function:

$$
\text{sgn}(x) = \frac{x}{|x|}
$$

## Properties of the Signum Function

1. **Odd Function**: The signum function is an odd function, meaning that $\text{sgn}(-x) = -\text{sgn}(x)$ for all $x$.

2. **Differentiability**: The signum function is not differentiable at $x = 0$, as it has a sharp corner at that point.

3. **[[Integral]] Representation**: The signum function can be represented as an [[integral]]:

$$
\text{sgn}(x) = \frac{1}{2\pi i}\int_{-\infty}^{\infty}\frac{\exp(iz)}{z-x}\,dz
$$

4. **[[Derivative]] Distribution**: The [[derivative]] of the signum function can be expressed using the [[Dirac delta function]]:

$$
\frac{{d\text{sgn}(x)}}{{dx}} = 2\delta(x)
$$

## Examples

**Example 1**: Find the value of $\text{sgn}(-5)$.

Solution:
Since $-5$ is negative, we have $\text{sgn}(-5) = -1$.

**Example 2**: Evaluate $\frac{d\text{sgn}(x)}{dx}$.

Solution:
The [[derivative]] of the signum function is given by $\frac{d\text{sgn}(x)}{dx} = 2\delta(x)$.

**Example 3**: Calculate the [[integral]] $\int_{-\infty}^{\infty}\text{sgn}(x)\,dx$.

Solution:
Since the signum function changes sign at $x = 0$, the [[integral]] evaluates to zero:

$$
\int_{-\infty}^{\infty}\text{sgn}(x)\,dx = 0
$$

## Key Theorems

**Theorem 1**: The signum function is discontinuous at $x = 0$.

**Proof**: To prove this theorem, we can consider the left and right limits of the signum function as $x$ approaches $0$. From the definition of the signum function, we have:

$$
\lim_{{x \to 0^-}} \text{sgn}(x) = -1 \quad \text{(left limit)}
$$

and

$$
\lim_{{x \to 0^+}} \text{sgn}(x) = 1 \quad \text{(right limit)}
$$

Since the left and right limits are not equal, $\text{sgn}(x)$ is discontinuous at $x = 0$.

**Theorem 2**: The [[derivative]] of the signum function is given by $\frac{{d\text{sgn}(x)}}{{dx}} = 2\delta(x)$.

**Proof**: To prove this theorem, we can use the definition of the [[derivative]] and evaluate it for different values of $x$. For $x < 0$, we have $\text{sgn}(x) = -1$, and for $x > 0$, we have $\text{sgn}(x) = 1$. Therefore, the [[derivative]] is zero everywhere except at $x = 0$, where it is infinite. This behavior can be represented using the [[Dirac delta function]]:

$$
\frac{{d\text{sgn}(x)}}{{dx}} = 2\delta(x)
$$

## Conclusion

The signum function is a useful mathematical tool for determining the sign of a real number. It has several properties and can be represented using integrals and derivatives. Understanding the signum function is important in various areas of mathematics, including calculus and signal processing.