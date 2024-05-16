#math 

Euler's formula is a fundamental result in mathematics that relates the exponential function, complex numbers, and trigonometry. It states that for any real number $x$, we have:

$$e^{ix} = \cos(x) + i\sin(x)$$

where $e$ is the base of the natural logarithm, $i$ is the imaginary unit, $\cos(x)$ represents the cosine function, and $\sin(x)$ represents the sine function.

## Derivation

To derive Euler's formula, we start with the [[Taylor series]] expansions of $e^{ix}$, $\cos(x)$, and $\sin(x)$:

$$e^{ix} = 1 + ix + \frac{(ix)^2}{2!} + \frac{(ix)^3}{3!} + \frac{(ix)^4}{4!} + \cdots$$

$$\cos(x) = 1 - \frac{x^2}{2!} + \frac{x^4}{4!} - \frac{x^6}{6!} + \cdots$$

$$\sin(x) = x - \frac{x^3}{3!} + \frac{x^5}{5!} - \frac{x^7}{7!} + \cdots$$

We can observe that in each series expansion, there are alternating terms with powers of $i$. By grouping these terms together, we can rewrite them as:

$$e^{ix} = (1 - \frac{x^2}{2!} + \frac{x^4}{4!} - \frac{x^6}{6!} + \cdots) + i(x - \frac{x^3}{3!} + \frac{x^5}{5!}-\frac{x^7}{7!})$$

Comparing this expression with the [[Taylor series]] expansions of $\cos(x)$ and $\sin(x)$, we can see that the real part of $e^{ix}$ matches with $\cos(x)$ and the imaginary part matches with $\sin(x)$. Therefore, we have derived Euler's formula:

$$e^{ix} = \cos(x) + i\sin(x)$$

## Implications

Euler's formula has profound implications in various branches of mathematics. Some key implications include:

### 1. Euler's Identity

Setting $x = \pi$ in Euler's formula yields Euler's identity:

$$e^{i\pi} + 1 = 0$$

This equation connects five fundamental mathematical constants: $e$, $i$, $\pi$, 0, and 1. It is considered one of the most beautiful equations in mathematics due to its simplicity and elegance.

### 2. Relationship between Trigonometry and Complex Exponentials

Euler's formula provides a deep connection between trigonometric functions and complex exponentials. By expressing trigonometric functions as complex exponentials, many trigonometric identities can be derived more easily using algebraic manipulations.

For example, we can express $\cos(2x+1)$ and $\sin(2x+1)$ in terms of complex exponentials as follows:

$$\cos(2x+1) = \frac{e^{i(2x+1)} + e^{-i(2x+1)}}{2}$$

$$\sin(2x+1) = \frac{e^{i(2x+1)} - e^{-i(2x+1)}}{2i}$$

### 3. Geometric Interpretation

Euler's formula also has a geometric interpretation on the complex plane. The exponential function $e^{ix}$ corresponds to a point on the unit circle in the complex plane, with an angle of $x$ radians from the positive real axis.

The real part of $e^{ix}$, $\cos(x)$, gives the x-coordinate of the point, while the imaginary part, $\sin(x)$, gives the y-coordinate. Thus, Euler's formula allows us to represent complex numbers in polar form.

## Example

Let's consider an example to illustrate the usefulness of Euler's formula. Suppose we want to evaluate the [[integral]]:

$$\int_0^\pi e^{ix} \ dx$$

Using Euler's formula, we can rewrite the integrand as:

$$\int_0^\pi (\cos(x) + i\sin(x)) \ dx$$

Splitting this into two separate integrals:

$$\int_0^\pi \cos(x) \ dx + i\int_0^\pi \sin(x) \ dx$$

Evaluating each [[integral]] separately:

$$[\sin(x)]_0^\pi + i[-\cos(x)]_0^\pi$$

Simplifying further:

$$(\sin(\pi) - \sin(0)) + i(-\cos(\pi) + \cos(0))$$

Since $\sin(\pi) = 0$ and $\cos(\pi) = -1$, we have:

$$0 - 1 + i(-(-1) + 1) = -1 + 2i$$

Thus, we have evaluated the [[integral]] using Euler's formula.

In conclusion, Euler's formula is a powerful mathematical result that connects exponential functions, complex numbers, and trigonometry. It has numerous applications in various areas of mathematics and provides deeper insights into these fundamental concepts.