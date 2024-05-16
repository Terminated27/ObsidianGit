

# Signal Additivity

In signal processing, additivity refers to the property of a system where the output resulting from the sum of multiple input signals is equal to the sum of the outputs produced by each individual input signal. Mathematically, this can be expressed as:

$$
f(x_1 + x_2) = f(x_1) + f(x_2)
$$

where $f$ is the system or function under consideration, and $x_1$ and $x_2$ are input signals.

## Key Theorems

### [[Superposition]] Theorem
The [[superposition]] theorem states that in a linear system, the response to a sum of multiple inputs is equal to the sum of the responses to each individual input. Mathematically, this can be expressed as:

$$
f(a \cdot x_1 + b \cdot x_2) = a \cdot f(x_1) + b \cdot f(x_2)
$$

where $a$ and $b$ are constants.

## Step-by-Step Example

Consider a system with the following response function:

$$
f(x) = 3x^2 - 5x + 7
$$

If we have two input signals $x_1 = 2$ and $x_2 = -3$, we can calculate the output for each signal separately:

For $x_1 = 2$:
$$
f(2) = 3(2)^2 - 5(2) + 7 = 12 - 10 + 7 = 9
$$

For $x_2 = -3$:
$$
f(-3) = 3(-3)^2 - 5(-3) + 7 = 27 +15 +7 =49
$$

Now, using additivity, we can calculate the output for the combined input signal $x_1 + x_2$:
$$
f(2+(-3))= f(-1)=3(-1)^{^} -5(-1)+7=-8+5+7=4 
$$

Therefore, by applying signal additivity, we get:

$$
f(2-3)=4=f(2)+f(-3)
$$