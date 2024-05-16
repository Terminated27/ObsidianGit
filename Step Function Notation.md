

# [[Step Function]] Notation

[[Step function]] notation is a mathematical notation used to represent functions that have a constant value over specific intervals. These functions are also known as "piecewise constant" or "discrete" functions. In this atomic note, we will explore the key concepts, theorems, and examples related to [[step function]] notation.

## Definition

A [[step function]] is defined as a function that takes on different constant values over different intervals. It can be represented using the [[step function]] notation as follows:

$$
f(x) = \begin{cases}
c_1 & \text{if } x < a_1 \\
c_2 & \text{if } a_1 \leq x < a_2 \\
\vdots \\
c_n & \text{if } a_{n-1} \leq x < a_n \\
\end{cases}
$$

where $c_1, c_2, ..., c_n$ are constants representing the values of the function over each interval $[a_i, a_{i+1})$.

## Properties and Theorems

### Jump Discontinuity

A [[step function]] is characterized by jump discontinuities at each $x = a_i$. At these points, the value of the function changes abruptly from one constant to another.

### [[Integral]] of Step Functions

The [[integral]] of a [[step function]] can be calculated by summing up the areas of rectangles formed by each constant value over its respective interval. Mathematically, if $F(x)$ is an antiderivative of $f(x)$ (the [[step function]]), then:

$$
\int f(x) dx = F(x) + C = \sum_{i=1}^{n} c_i (x - a_i)
$$

where $C$ is the constant of [[integration]].

### [[Derivative]] of Step Functions

The [[derivative]] of a [[step function]] is zero almost everywhere, except at the jump discontinuities. At these points, the [[derivative]] has a "spike" or "impulse" of height equal to the difference in values between the two adjacent constants.

## Step-by-Step Examples

### Example 1

Consider the [[step function]] defined as:

$$
f(x) = \begin{cases}
2 & \text{if } x < 0 \\
-1 & \text{if } 0 \leq x < 2 \\
3 & \text{if } x \geq 2 \\
\end{cases}
$$

Plotting this [[step function]], we can see that it takes on different constant values over different intervals.

```
   |   3
   |
---|--------
   |
 -1|
---|--------
   |       2
```

### Example 2

Let's calculate the [[integral]] of the [[step function]] defined in Example 1 over the interval $[0, 4]$.

First, we find an antiderivative $F(x)$ of $f(x)$:
$$
F(x) = \begin{cases}
2x & \text{if } x < 0 \\
-1x & \text{if } 0 \leq x < 2 \\
3x & \text{if } x \geq 2 \\
\end{cases}
$$

Now, we can calculate the definite [[integral]]:
$$
\int_0^4 f(x) dx = F(4) - F(0) = (3)(4) - (-1)(2) + (2)(0) = 14
$$

Thus, the [[integral]] of the [[step function]] over $[0, 4]$ is equal to $14$.

## Conclusion

[[Step function]] notation provides a concise way to represent functions with constant values over specific intervals. These functions have jump discontinuities and their integrals can be calculated by summing up the areas of rectangles formed by each constant value. The [[derivative]] of a [[step function]] is zero almost everywhere, except at the jump discontinuities where it has a spike.