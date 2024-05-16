#Conttime 

S-domain analysis is a powerful tool used in electrical engineering to analyze linear time-invariant circuits in the frequency domain. It involves transforming the circuit from the time domain to the [[Laplace domain]] using the [[Laplace transform]]. This transformation simplifies the analysis of circuits by allowing us to work with algebraic equations instead of differential equations.

## Key Theorems and Definitions

### [[Laplace Transform]]
The [[Laplace transform]] of a function $f(t)$ is defined as:
$$ F(s) = \mathcal{L}\{f(t)\} = \int_{0}^{\infty} e^{-st} f(t) dt $$

### [[Transfer Function]]
The [[transfer function]] of a circuit is defined as the ratio of the [[Laplace transform]] of the output to the [[Laplace transform]] of the input, assuming zero initial conditions:
$$ H(s) = \frac{V_{\text{out}}(s)}{V_{\text{in}}(s)} $$

### Poles and Zeros
Poles are values of $s$ for which the [[transfer function]] becomes infinite, while zeros are values of $s$ for which the [[transfer function]] becomes zero.

## Step-by-Step Example

Let's consider a simple RC circuit with a [[voltage]] source $V_{\text{in}}(t)$ and a [[resistor]] $R$ in series with a capacitor $C$. The [[voltage]] across the capacitor is denoted as $V_{\text{out}}(t)$.

1. Apply [[Kirchhoff's voltage law]] to write down the [[differential equation]] governing this circuit:
$$ V_{\text{in}}(t) - R I(t) - \frac{1}{C} \int I(t) dt = 0 $$

2. Take the [[Laplace transform]] of this equation to obtain an algebraic equation in terms of $I(s)$ and $V_{\text{in}}(s)$:
$$ V_{\text{in}}(s) - R I(s) - \frac{1}{Cs} I(s) = 0 $$

3. Solve for $I(s)$ in terms of $V_{\text{in}}(s)$ and find the [[transfer function]]:
$$ H(s) = \frac{V_{\text{out}}(s)}{V_{\text{in}}(s)} = \frac{\frac{1}{Cs}}{\frac{R}{Cs} + 1} = \frac{1}{RCs + 1} $$

4. Analyze the poles and zeros of this [[transfer function]] to understand its behavior in the frequency domain.

By performing S-domain circuit analysis, we can gain valuable insights into how circuits respond to continuous time signals and design systems that meet specific performance requirements.