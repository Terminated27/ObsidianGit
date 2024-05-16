#calculus #math 

In calculus, the integral is a fundamental concept that represents the area under a curve or the accumulation of a quantity. It is denoted by the symbol $\int$, and it has various applications in mathematics and science.

## Definite Integral

The definite integral of a function $f(x)$ over an interval $[a, b]$ is defined as the limit of Riemann sums as the partition size approaches zero. It represents the net signed area between the curve and the x-axis over that interval. The definite integral is denoted as follows:

$$\int_{a}^{b} f(x) \ dx$$

### Properties of Definite Integrals

1. **Linearity**: For any functions $f(x)$ and $g(x)$, and constants $c_1$ and $c_2$, we have:

   $$\int_{a}^{b} (c_1f(x) + c_2g(x)) \ dx = c_1\int_{a}^{b} f(x) \ dx + c_2\int_{a}^{b} g(x) \ dx$$

2. **Additivity**: If $c$ lies between $a$ and $b$, then:

   $$\int_{a}^{b} f(x) \ dx = \int_{a}^{c} f(x) \ dx + \int_{c}^{b} f(x) \ dx$$

3. **Change of Limits**: If $\phi$ is a continuously differentiable function on $[p, q]$ such that $\phi(p) = a$ and $\phi(q) = b$, then:

   $$\int_{a}^{b} f(x) \ dx = \int_{p}^{q}(f(\phi(t))\phi'(t)) \ dt$$


## Indefinite Integral

The indefinite integral of a function $f(x)$ represents the antiderivative or primitive of $f(x)$. It is denoted as follows:

$$\int f(x) \ dx$$

### Properties of Indefinite Integrals

1. **[[Linearity]]**: For any functions $f(x)$ and $g(x)$, and constants $c_1$ and $c_2$, we have:

   $$\int (c_1f(x) + c_2g(x)) \ dx = c_1\int f(x) \ dx + c_2\int g(x) \ dx$$

2. **[[Power Rule]]**: For any real number $n \neq -1$, we have:

   $$\int x^n \ dx = \frac{x^{n+1}}{n+1} + C$$

   where $C$ is the constant of [[integration]].

3. **[[Integration by Parts]]**: If $u$ and $v$ are differentiable functions, then:

   $$\int u \ dv = uv - \int v \ du$$


## [[Fundamental Theorem of Calculus]]

The [[fundamental theorem of calculus]] establishes the connection between differentiation and [[integration]]. It consists of two parts.
