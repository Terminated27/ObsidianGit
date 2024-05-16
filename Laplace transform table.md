#math #diffeq 

The [[Laplace transform]] is a mathematical tool used to solve [[linear]] ordinary differential equations. It transforms a function of time into a function of complex frequency, making it easier to analyze and solve differential equations. The [[Laplace transform]] of a function $f(t)$ is denoted by $\mathcal{L}\{f(t)\}$ or $F(s)$, where $s$ is the complex frequency.

## Definition

The [[Laplace transform]] of a function $f(t)$ is defined as:

$$\mathcal{L}\{f(t)\} = F(s) = \int_{0}^{\infty} e^{-st} f(t) dt$$

where $s = \sigma + j\omega$ is the complex frequency, with $\sigma$ being the real part and $\omega$ being the imaginary part.

## Key Theorems

### Linearity

The [[Laplace transform]] satisfies the linearity property:

$$\mathcal{L}\{af(t) + bg(t)\} = aF(s) + bG(s)$$

where $a$ and $b$ are constants, and $F(s)$ and $G(s)$ are the Laplace transforms of functions $f(t)$ and $g(t)$ respectively.

### Time Shifting

If $\mathcal{L}\{f(t)\} = F(s)$, then for any positive constant $a$, we have:

$$\mathcal{L}\{f(t-a)\} = e^{-as}F(s)$$

### Frequency Shifting

If $\mathcal{L}\{f(t)\} = F(s)$, then for any positive constant $\omega$, we have:

$$\mathcal{L}\{e^{\omega t} f(t)\} = F(s-j\omega)$$

### Differentiation in Time Domain

If $\mathcal{L}\{f(t)\} = F(s)$, then:

$$\mathcal{L}\{\frac{{df(t)}}{{dt}}\} = sF(s) - f(0)$$

### [[Integration]] in Time Domain

If $\mathcal{L}\{f(t)\} = F(s)$, then:

$$\mathcal{L}\{\int_{0}^{t} f(\tau) d\tau\} = \frac{{F(s)}}{{s}}$$

## [[Laplace Transform]] Table


Here is a table of some common functions and their Laplace transforms:
more @ [[laplace-table.pdf]]

| Function $f(t)$ | [[Laplace Transform]] $F(s)$ |
|-----------------|-------------------------|
| $1$             | $\frac{1}{s}$           |
| $t^n$           | $\frac{n!}{s^{n+1}}$    |
| $e^{at}$        | $\frac{1}{s-a}$         |
| $\sin(\omega t)$   | $\frac{\omega}{s^2+\omega^2}$      |
| $\cos(\omega t)$   | $\frac{s}{s^2+\omega^2}$      |
| $u(t-a)$        | $\frac{e^{-as}}{s}$     |

where $n$ is a positive integer and $a$ is a constant.

