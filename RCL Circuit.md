#diffeq #math #physics #hardware 

**Introduction:**
RCL circuits, consisting of resistors (R), capacitors (C), and inductors (L), are fundamental components in electrical engineering. Analyzing these circuits often involves solving differential equations. This atomic note outlines the essential steps to solve RCL circuits using differential equations.

**Steps:**

1. **Kirchhoff's [[Voltage]] Law (KVL):** Apply KVL to the circuit to derive the governing [[Differential Equation]]. The sum of [[voltage]] drops in any closed loop of the circuit must be equal to the electromotive force (EMF) supplied.

   **$$V(t) = L\frac{di(t)}{dt} + Ri(t) + \frac{1}{C}\int i(t) dt$$**

   Here, $V(t)$ represents the applied [[voltage]], $L$ is the inductance, $R$ is the resistance, $C$ is the [[capacitance]], and $i(t)$ is the [[current]] as a function of time.

2. **Solve the [[Differential Equation]]:** Solve the derived [[Differential Equation]] using appropriate techniques (e.g., separation of variables, integrating factors, or Laplace transforms) to find the expression for [[current]] ($i(t)$) as a function of time.

3. **Initial Conditions:** Apply any given initial conditions, such as the initial [[current]] or [[voltage]] across the components, to determine the constants of [[integration]] in the solution.

4. **Interpret the Solution:** Analyze the solution to understand the behavior of the circuit. Determine how the [[current]] and [[voltage]] across the components vary with time, considering the circuit's specific characteristics.

5. **Steady State Analysis (Optional):** For AC circuits, analyze the steady-state behavior, typically after transient effects have decayed. Express the solution in terms of phasors and identify the amplitude, [[phase]], and frequency of the [[current]] and [[voltage]] waveforms.

6. **Verification and Comparison:** Verify the obtained solution by checking against known results or comparing with simulations. Ensure that the solution aligns with the expected behavior of the RCL circuit under consideration.

**Conclusion:**
Solving RCL circuits using differential equations is a crucial skill in electrical engineering. By applying Kirchhoff's laws and appropriate techniques to the governing equation, one can obtain valuable insights into the circuit's behavior, aiding in the design and analysis of complex electrical systems.

# [[Characteristic Equation]] method

**Step 1: Formulate the [[Differential Equation]]:**
Start with Kirchhoff's [[voltage]] law (KVL) for the RLC circuit, which results in a second-[[order]] [[linear]] homogeneous [[Differential Equation]]. For instance, the general form of the equation for a series RLC circuit with a [[voltage source]] $V(t)$ is:

$$ L\frac{d^2i(t)}{dt^2} + R\frac{di(t)}{dt} + \frac{1}{C}i(t) = V(t) $$

**Step 2: Find the [[Characteristic Equation]]:**
Assume a solution of the form $i(t) = Ae^{rt}$, where $A$ is a constant and $r$ is an unknown parameter. Substitute this solution into the [[Differential Equation]]:

$$ Lr^2e^{rt} + Rre^{rt} + \frac{1}{C}e^{rt} = 0 $$

Factor out the exponential term:

$$ e^{rt} (Lr^2 + Rr + \frac{1}{C}) = 0 $$

For a non-trivial solution ($e^{rt} \neq 0$), the expression in the parentheses must be equal to zero. This gives you the [[characteristic equation]]:

$$ Lr^2 + Rr + \frac{1}{C} = 0 $$

**Step 3: Solve the [[Characteristic Equation]]:**
Solve the [[characteristic equation]] to find the values of $r$. These values represent the roots of the [[characteristic equation]] and are called the eigenvalues. Depending on the nature of the roots (real, complex, or repeated), the [[general solution]] for $i(t)$ can be expressed as a combination of exponential functions, sines, and cosines.

**Step 4: Apply Initial Conditions (if any):**
If initial conditions for [[current]] ($i(0)$) and its [[Derivative]] ($di(0)/dt$) are given, use them to determine the constants in the [[general solution]].

By following these steps, you can solve RLC circuits using the [[characteristic equation]] method, providing a systematic approach to find the response of the circuit to different input conditions.

## example

Let's consider a specific example of a series RLC circuit with the following parameters:

- Resistance ($R$): $2 \, \Omega$
- Inductance ($L$): $1 \, \text{H}$
- [[Capacitance]] ($C$): $0.5 \, \text{F}$
- Applied [[Voltage]] ($V(t)$): $5 \cos(2t)$

We'll use the [[characteristic equation]] method to find the solution for the [[current]] ($i(t)$) in the circuit.

**Step 1:** Formulate the [[Differential Equation]]:

$$ L\frac{d^2i(t)}{dt^2} + R\frac{di(t)}{dt} + \frac{1}{C}i(t) = 5 \cos(2t) $$

**Step 2:** Find the [[Characteristic Equation]]:

The [[characteristic equation]] for this circuit is:

$$ Lr^2 + Rr + \frac{1}{C} = 0 $$
$$ r^2 + 2r + 2 = 0 $$

**Step 3:** Solve the [[Characteristic Equation]]:

Using the [[quadratic formula]], we find the roots ($r$):

$$ r = \frac{-2 \pm \sqrt{(-2)^2 - 4(1)(2)}}{2(1)} $$
$$ r = -1 \pm i\sqrt{3} $$

The roots are complex ($r_1 = -1 + i\sqrt{3}$ and $r_2 = -1 - i\sqrt{3}$).

**Step 4:** [[General Solution]]:

The [[general solution]] for the [[current]] ($i(t)$) in the circuit is:

$$ i(t) = e^{-t}(A\cos(\sqrt{3}t) + B\sin(\sqrt{3}t)) $$

**Step 5:** Apply Initial Conditions (if any):

If initial conditions are given (for example, $i(0) = 1$ A and $\frac{di(0)}{dt} = 0$), substitute them into the [[general solution]] to find the constants $A$ and $B$.

Using $i(0) = 1$, we get:

$$ 1 = A $$

Using $\frac{di(0)}{dt} = 0$, we find $\frac{di(t)}{dt} = -\sqrt{3}Ae^{-t}\sin(\sqrt{3}t)$. At $t = 0$, this equals 0, so $B = 0$.

**Conclusion:**

The solution for the [[current]] in the RLC circuit with the given parameters and applied [[voltage]] is:

$$ i(t) = e^{-t}\cos(\sqrt{3}t) $$
# example

Let's consider a simple series RLC circuit connected to a DC [[voltage]] source. In this example, we'll assume a DC [[voltage]] source $ V = 10 \, \text{V} $ and the following circuit parameters:

- Resistance ($ R $): $ 3 \, \Omega $
- Inductance ($ L $): $ 2 \, \text{H} $
- [[Capacitance]] ($ C $): $ 1 \, \text{F} $

**Step 1:** Apply Kirchhoff's [[Voltage]] Law (KVL) to the circuit to obtain the [[Differential Equation]]. For a DC circuit, the equation simplifies to:

$$ V = L\frac{di(t)}{dt} + Ri(t) + \frac{1}{C}\int i(t) dt $$

Substituting the given values, the equation becomes:

$$ 10 = 2\frac{di(t)}{dt} + 3i(t) + \frac{1}{1}\int i(t) dt $$

**Step 2:** Solve this first-[[order]] [[linear]] [[ordinary differential equation]] to find $ i(t) $, the [[current]] flowing through the circuit.

**Step 3:** Apply any initial conditions if provided (for example, $ i(0) = 0 $ A).

**Step 4:** Interpret the solution, which represents how the [[current]] in the circuit changes over time under the given DC [[voltage]] source and circuit parameters. The solution might involve exponential functions due to the presence of both inductive and resistive components.

To solve the [[Differential Equation]], you can use techniques like separation of variables or integrating factors. The exact solution will depend on the form of the applied DC [[voltage]] and any initial conditions specified.

Certainly! Let's solve the given first-[[order]] [[linear]] ordinary [[Differential Equation]] for the series RLC circuit with the specified parameters and DC [[voltage source]] ($ V = 10 \, \text{V} $):

$$ 10 = 2\frac{di(t)}{dt} + 3i(t) + \int i(t) dt $$

To solve this equation, we first need to find the particular solution and the homogeneous solution.

**Homogeneous Solution:**
The homogeneous part of the solution is obtained by setting the right-hand side to zero:

$$ 2\frac{di_h(t)}{dt} + 3i_h(t) = 0 $$

This is a [[linear]] homogeneous first-[[order]] [[Differential Equation]]. Solving it, we get:

$$ i_h(t) = Ae^{-\frac{3}{2}t} $$

where $ A $ is an arbitrary constant.

**Particular Solution:**
For the particular solution, we assume a constant [[current]] ($ i_p $) since the source is DC (constant [[voltage]]):

$$ 2\frac{di_p}{dt} + 3i_p = 0 $$

Solving this, we find $ i_p = -\frac{3}{2} $.

**Complete Solution:**
The complete solution is the sum of the homogeneous and particular solutions:

$$ i(t) = i_h(t) + i_p = Ae^{-\frac{3}{2}t} - \frac{3}{2} $$

**Applying [[Initial Condition]]:**
If an [[initial condition]] is provided, say $ i(0) = I_0 $, we can substitute this into the equation to find the value of $ A $:

$$ I_0 = A - \frac{3}{2} $$
$$ A = I_0 + \frac{3}{2} $$

So, the final solution for the [[current]] ($ i(t) $) in the circuit with the given DC [[voltage source]] and [[initial condition]] is:

$$ i(t) = \left(I_0 + \frac{3}{2}\right)e^{-\frac{3}{2}t} - \frac{3}{2} $$

This equation represents the [[current]] flowing through the circuit as a function of time under the specified conditions.