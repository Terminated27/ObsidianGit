#diffeq #math 
When guessing a particular solution for a nonhomogeneous second-[[order]] [[ordinary differential equation]] ([[ODE]]) with constant coefficients, the form of the guess depends on the form of the nonhomogeneous term. Here are some common forms of nonhomogeneous terms and their corresponding guesses for the particular solution:

if not then try these:

1. **For $F(x) = Ae^{mx}$ (exponential function):**
   - Guess: $y_p(x) = Be^{mx}$
   - Note: If $e^{mx}$ is part of the homogeneous solution, multiply the guess by $x$ or $x^2$ until the guess is no longer in the homogeneous solution.

2. **For $F(x) = A\cos(mx) + B\sin(mx)$ (trigonometric functions):**
   - Guess: $y_p(x) = C\cos(mx) + D\sin(mx)$
   - Note: If $\cos(mx)$ or $\sin(mx)$ is part of the homogeneous solution, multiply the guess by $x$ or $x^2$ until the guess is no longer in the homogeneous solution.

3. **For $F(x) = P_n(x)e^{mx}$ (polynomial multiplied by an exponential term):**
   - Guess: $y_p(x) = Q_n(x)e^{mx}$, where $Q_n(x)$ is a polynomial of the same degree as $P_n(x)$.
   - Note: Determine the degree of the polynomial part based on the degree of $P_n(x)$. If $e^{mx}$ is part of the homogeneous solution, multiply the guess by $x$ or $x^2$ until the guess is no longer in the homogeneous solution.

4. **For $F(x) = P_n(x)$ (polynomial only):**
   - Guess: $y_p(x) = Q_n(x)$, where $Q_n(x)$ is a polynomial of the same degree as $P_n(x)$.
   - Note: If any term in the guess is already part of the homogeneous solution, multiply the guess by $x$ or $x^2$ until the guess is no longer in the homogeneous solution.

5. **For $F(t) = 6t^n$ (polynomial function of $t$):**

 a. **If $n$ is not an integer:**
   - **Guess:** $y_p(t) = At^n + Bt^{n+1} + \ldots + Kt^{n+k}$
   - **Note:** Here, $A$, $B$, $K$, etc., are constants to be determined. Include terms up to the highest [[power]] needed to match the degree of the nonhomogeneous term. If $t^n$ is part of the homogeneous solution, multiply the guess by $t$ or $t^2$ until the guess is no longer in the homogeneous solution.

 b. **If $n$ is an integer:**
   - **Guess:** $y_p(t) = At^n$
   - **Note:** Here, $A$ is a constant to be determined. Include the term $t^n$ in the guess. If $t^n$ is part of the homogeneous solution, multiply the guess by $t$ or $t^2$ until the guess is no longer in the homogeneous solution.

6. **For $F(x) = mx + b$ (linear function of $x$):**
   - **Guess:** $y_p(x) = Mx + N$
   - **Note:** Here, $M$ and $N$ are constants to be determined. If $x$ is already part of the homogeneous solution, multiply the guess by $x$ or $x^2$ until the guess is no longer in the homogeneous solution.

