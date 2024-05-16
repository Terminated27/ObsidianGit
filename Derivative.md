#calculus #math
## Introduction

The derivative is a fundamental concept in calculus that measures the rate of change of a function with respect to its independent variable. It is denoted by $f'(x)$ or $\frac{df}{dx}$ and represents the slope of the tangent line to the graph of the function at a given point. The derivative has many applications in mathematics, physics, economics, and other fields.

## Definition

The derivative of a function $f(x)$ at a point $x=a$ is defined as:

$$
f'(a) = \lim_{h \to 0} \frac{f(a+h) - f(a)}{h}
$$

This limit represents the instantaneous rate of change of $f(x)$ at $x=a$. When this limit exists, we say that $f(x)$ is differentiable at $x=a$.

## Basic Rules

There are several rules for finding derivatives that make it easier to calculate them. These include:

1. **[[Power Rule]]:** If $f(x) = x^n$, then $f'(x) = nx^{n-1}$.
2. **[[Product Rule]]:** If $f(x) = u(x)v(x)$, then $f'(x) = u'(x)v(x)+u(x)v'(x)$.
3. **Quotient Rule:** If $f(x) = \frac{u(x)}{v(x)}$, then $f'(x) = \frac{u'(x)v(x)-u(x)v'(x)}{(v(x))^2}$.
4. **Chain Rule:** If $g(x)$ is differentiable at $x$ and $h(u)$ is differentiable at $u=g(x)$, then $(h \circ g)'(x)= h'(g(x))g'(x)$.

## Key Theorems

### Mean Value Theorem

The Mean Value Theorem states that if $f(x)$ is continuous on the closed interval $[a,b]$ and differentiable on the [[open interval]] $(a,b)$, then there exists a point $c \in (a,b)$ such that:

$$
f'(c) = \frac{f(b)-f(a)}{b-a}
$$

This means that at some point in the interval, the instantaneous rate of change (derivative) is equal to the average rate of change over the entire interval.

### Rolle's Theorem

Rolle's Theorem is a special case of the Mean Value Theorem. It states that if $f(x)$ is continuous on $[a,b]$, differentiable on $(a,b)$, and $f(a)=f(b)$, then there exists a point $c \in (a,b)$ such that $f'(c)=0$. In other words, there is at least one point in the interval where the tangent line is horizontal.

## Examples

### Example 1: Finding Derivatives using Basic Rules

Find the derivative of $f(x) = 3x^2-5x+2$.

**Solution:**

Using the [[power rule]], we have:

$$
\begin{align*}
f'(x) &= 3(2)x^{2-1}-5(1)x^{1-1}+0 \\
&= 6x-5
\end{align*}
$$

### Example 2: Applying Chain Rule

Find the derivative of $g(x) = (4x^3+7)^4$.

**Solution:**

Using chain rule, we have:

$$
\begin{align*}
g'(x) &= 4(4x^3+7)^3(12x^2)+0 \\
&= 48x^2(4x^3+7)^3
\end{align*}
$$

## Conclusion

The derivative is a powerful tool in calculus that allows us to analyze the behavior of functions and solve various problems. It is important to understand the definition, basic rules, and key theorems related to derivatives in order to apply them effectively. With practice, finding derivatives becomes easier and more intuitive. 