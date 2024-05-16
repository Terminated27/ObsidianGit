#diffeq #math 
The Inverse [[Laplace Transform]] is an operation that allows us to recover a function from its [[Laplace transform]]. It is denoted by the symbol $\mathcal{L}^{-1}$.
Also see: [[laplace-table.pdf]]
## Definition

Given a function $F(s)$, the inverse [[Laplace transform]] of $F(s)$ is denoted as $\mathcal{L}^{-1}\{F(s)\}$ and is defined as:

$$
f(t) = \mathcal{L}^{-1}\{F(s)\} = \frac{1}{2\pi i}\lim_{T\to\infty}\int_{\gamma-iT}^{\gamma+iT}e^{st}F(s)ds
$$

where $\gamma$ is a constant such that the line of [[integration]] lies to the right of all singularities of $F(s)$.

## Key Theorems

### Linearity Property

If $F_1(s)$ and $F_2(s)$ are the Laplace transforms of functions $f_1(t)$ and $f_2(t)$ respectively, and $a$ and $b$ are constants, then the inverse [[Laplace transform]] of $aF_1(s) + bF_2(s)$ is given by:

$$
\mathcal{L}^{-1}\{aF_1(s) + bF_2(s)\} = a\mathcal{L}^{-1}\{F_1(s)\} + b\mathcal{L}^{-1}\{F_2(s)\}
$$

### Shifting Property

If $F(s)$ is the [[Laplace transform]] of a function $f(t)$, then for any positive constant $a$, the inverse [[Laplace transform]] of $e^{-as} F(as)$ is given by:

$$
\mathcal{L}^{-1}\{e^{-as} F(as)\} = f(t-a)
$$

### [[Convolution]] Property

If $F_1(s)$ and $F_2(s)$ are the Laplace transforms of functions $f_1(t)$ and $f_2(t)$ respectively, then the inverse [[Laplace transform]] of their product $F_1(s)F_2(s)$ is given by:

$$
\mathcal{L}^{-1}\{F_1(s)F_2(s)\} = \int_{0}^{t}f_1(\tau)f_2(t-\tau)d\tau
$$

## Examples

**Example 1:**

Find the inverse [[Laplace transform]] of $\frac{s}{s^2+4}$.

**Solution:**

We can rewrite the given function as:

$$
\frac{s}{s^2+4} = \frac{s}{(s+2i)(s-2i)}
$$

Using partial fractions, we can express it as:

$$
\frac{s}{(s+2i)(s-2i)} = \frac{A}{s+2i} + \frac{B}{s-2i}
$$

Multiplying both sides by $(s+2i)(s-2i)$, we get:

$$
s = A(s-2i) + B(s+2i)
$$

Expanding and equating coefficients, we find that $A= \frac{1}{4i}$ and $B= -\frac{1}{4i}$.

Therefore, the inverse [[Laplace transform]] is given by:

$$
\mathcal{L}^{-1}\left\{\frac{s}{s^2+4}\right\} = \mathcal{L}^{-1}\left\{\frac{\frac{1}{4i}}{s+2i} - \frac{\frac{1}{4i}}{s-2i}\right\} = \frac{1}{4i}\mathcal{L}^{-1}\left\{\frac{1}{s+2i}\right\} - \frac{1}{4i}\mathcal{L}^{-1}\left\{\frac{1}{s-2i}\right\}
$$

Using the shifting property, we have:

$$
\mathcal{L}^{-1}\left\{\frac{s}{s^2+4}\right\} = \frac{1}{4i}(e^{-2it}) - \frac{1}{4i}(e^{2it}) = \sin(2t)
$$

Therefore, the inverse [[Laplace transform]] of $\frac{s}{s^2+4}$ is $\sin(2t)$.
