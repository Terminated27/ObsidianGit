

The Euclidean Algorithm is an efficient method for finding the greatest common divisor (GCD) of two integers. It is based on the following key theorem:

**Theorem:** For any two non-negative integers $a$ and $b$, where $a > b$, the GCD of $a$ and $b$ is equal to the GCD of $b$ and the remainder of $a$ divided by $b.

This theorem forms the basis for the step-by-step process of the Euclidean Algorithm:

1. **Step 1:** Given two integers $a$ and $b$, where $a > b$, divide $a$ by $b$ to get a quotient $q_1$ and a remainder $r_1$. Write this as: $$ a = bq_1 + r_1 $$

2. **Step 2:** If the remainder $r_1 = 0$, then the GCD of $a$ and $b$ is equal to $b$. If not, proceed to the next step.

3. **Step 3:** [[Set]] $a = b$ and $b = r_1$, then repeat Step 1 with these new values.

4. **Step 4:** Continue this process until reaching a remainder of 0, at which point the last non-zero remainder will be the GCD of the original two integers.

Let's illustrate this algorithm with an example:

**Example:** Find the GCD of 48 and 18 using the Euclidean Algorithm.

- Step 1: $$48 = 18 \times 2 + 12$$
- Step 2: Since remainder $\neq 0$, proceed to next step.
- Step 3: Set $(48,18) \rightarrow (18,12)$
- Step 4: $$18 = 12 \times 1 +6$$
- Step 5: Set $(18,12) \rightarrow (12,6)$
- Step 6: $$12 =6 \times2+0$$

Since we have reached a remainder of zero, our final non-zero remainder is $\boxed{6}$, which is the GCD of 48 and 18.

The Euclidean Algorithm provides a systematic way to compute GCDs efficiently, making it a fundamental tool in number theory and cryptography.
![[Pasted image 20240306133411.png]]