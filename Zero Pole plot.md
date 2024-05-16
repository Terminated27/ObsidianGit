#Conttime 


In the study of continuous time signals, the zero pole plot is a graphical representation that provides insight into the behavior of a system. It shows the location of zeros and poles in the complex plane, which are crucial in understanding the stability and frequency response of a system.

## Definitions
- **Zeros**: Zeros are the values of \( s \) for which the [[transfer function]] becomes zero, i.e., \( H(s) = 0 \).
- **Poles**: Poles are the values of \( s \) for which the [[transfer function]] becomes infinite or undefined, i.e., \( H(s) = \infty \).

## Key Theorems
1. **Pole-Zero Plot Theorem**: For a rational [[transfer function]] \( H(s) = \frac{N(s)}{D(s)} \), where \( N(s) \) and \( D(s) \) are [[polynomials]] in \( s \), the zeros are the roots of \( N(s) = 0 \) and poles are the roots of \( D(s) = 0 \).
   
   $$ H(s) = K\frac{(s - z_1)(s - z_2)...(s - z_m)}{(s - p_1)(s - p_2)...(s - p_n)} $$

2. **Stability Criterion**: A system is stable if all its poles have negative real parts.

## Step-by-Step Example
Consider a system with [[transfer function]]:

$$ H(s) = K\frac{s + 2}{(s + 1)(s + 3)} $$

1. Identify zeros and poles:
   - Zeros: \( z = -2 \)
   - Poles: \( p_1 = -1, p_2 = -3 \)

2. Plot these points on the complex plane:
![[Pasted image 20240408102907.png]]
something like this, 0 is o and pole is x
3. Analyze stability:
   Since both poles have negative real parts, this system is stable.

By analyzing zero pole plots, we can gain valuable insights into the behavior and characteristics of continuous time signal systems.