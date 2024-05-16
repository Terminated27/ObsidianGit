 #math #stats 
![[Pasted image 20240304091731.png]]

The Cumulative Distribution Function (CDF) of a [[random variable]] X is defined as:

$$ F(x) = P(X \leq x) $$

where $F(x)$ gives the probability that the [[random variable]] X takes on a value less than or equal to x.

## Properties of CDF

1. **Non-decreasing**: The CDF is a non-decreasing function, i.e., for any $x_1 < x_2$, we have $F(x_1) \leq F(x_2)$.

2. **Right-continuous**: The CDF is right-continuous, meaning that $\lim_{h \to 0^+} F(x + h) = F(x)$ for all x.

3. **Limits at infinity**: $\lim_{x \to -\infty} F(x) = 0$ and $\lim_{x \to \infty} F(x) = 1$.

## Inverse CDF

The inverse of the CDF, denoted as $F^{-1}(p)$, gives the value x such that $F(x) = p$. It is useful in generating random variables with a specified distribution.

## Example

Let's consider a [[continuous random variable]] X with [[probability density function]]:

$$ f_X(x) = 
\begin{cases}
    2x & \text{for } 0 < x < 1 \\
    0 & \text{otherwise}
\end{cases}
$$

To find the CDF F(x), we integrate the PDF:

$$ F_X(x) = \int_{-\infty}^{x} f_X(t) dt $$

For $0 < x < 1$:

$$ F_X(x) = \int_{0}^{x} 2t dt = t^2 |_0^x = x^2 $$

Therefore, the CDF of X is:

$$ F_X(x) =
\begin{cases}
    0 & \text{for } x \leq 0 \\
    x^2 & \text{for } 0 < x < 1 \\
    1 & \text{for } x \geq 1
\end{cases}
$$