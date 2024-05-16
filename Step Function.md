#math

A step function, also known as a staircase function, is a mathematical function that takes on a constant value over each interval. It is defined by specifying the value of the function within each interval.
[[Step Function Notation]]
## Definition

A step function $f(x)$ is defined as follows:

$$
f(x) = \begin{cases} 
      c_1 & \text{if } x \in [a_1, b_1) \\
      c_2 & \text{if } x \in [a_2, b_2) \\
      \vdots \\
      c_n & \text{if } x \in [a_n, b_n) \\
   \end{cases}
$$

where $c_i$ is the constant value of the function within the interval $[a_i, b_i)$.

## Properties

1. **Discontinuities**: A step function has discontinuities at each point where the intervals change.
2. **Constant Intervals**: The step function remains constant within each interval.
3. **Jump Discontinuities**: At each point where the intervals change, there is a jump in the function value.

## Example

Consider the following step function:

$$
f(x) = \begin{cases} 
      0 & \text{if } x < 0 \\
      1 & \text{if } 0 \leq x < 1 \\
      -1 & \text{if } 1 \leq x < 2 \\
   \end{cases}
$$

In this example, $f(x)$ takes on different constant values within three intervals: $(-\infty, 0)$, $[0, 1)$, and $[1, 2)$. The [[Graph]] of this step function would consist of horizontal line segments connecting these constant values.

## Theorem: [[Integral]] of a Step Function

The [[integral]] of a step function $f(x)$ over an interval $[a, b]$ is given by:

$$
\int_a^b f(x) \, dx = \sum_{i=1}^n c_i \cdot (b_i - a_i)
$$

where $c_i$ is the constant value of $f(x)$ within the interval $[a_i, b_i)$.

## Proof

To prove this theorem, we divide the interval $[a, b]$ into subintervals based on the points where the intervals of the step function change. Within each subinterval, $f(x)$ is constant. Therefore, we can calculate the area under each constant segment and sum them up to obtain the total [[integral]].

Let's consider one such subinterval $[a_i, b_i)$. Within this subinterval, $f(x)$ takes on a constant value of $c_i$. The area under this constant segment is given by:

$$
\int_{a_i}^{b_i} f(x) \, dx = c_i \cdot (b_i - a_i)
$$

Summing up these areas for all subintervals gives us:

$$
\int_a^b f(x) \, dx = \sum_{i=1}^n c_i \cdot (b_i - a_i)
$$

which completes the proof.

## Conclusion

Step functions are useful mathematical tools for modeling situations where a quantity remains constant within specific intervals. They have interesting properties related to discontinuities and jump discontinuities. The [[integral]] of a step function can be calculated by summing up areas under each constant segment within the specified interval.