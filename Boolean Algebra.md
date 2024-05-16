
Boolean algebra is a branch of mathematics that deals with variables that can only take on two values: true (1) or false (0). It is widely used in computer science and digital electronics for designing circuits and analyzing logic gates.

## Basic Definitions

- **Variable**: A symbol representing a logical value, typically denoted by letters such as $A$, $B$, $C$, etc.
- **Constant**: Fixed logical values, typically denoted by 0 (false) and 1 (true).
- **Complement**: The negation of a variable, denoted by $\overline{A}$ or $A'$.
- **Conjunction**: The logical AND operation between two variables, denoted by $A \cdot B$ or $AB$.
- **Disjunction**: The logical OR operation between two variables, denoted by $A + B$.

## Key Theorems

1. **Idempotent Law**:
   - $A + A = A$
   - $A \cdot A = A$

2. **Commutative Law**:
   - $A + B = B + A$
   - $A \cdot B = B \cdot A$

3. **Associative Law**:
   - $(A + B) + C = A + (B + C)$
   - $(A \cdot B) \cdot C = A \cdot (B \cdot C)$

4. **Distributive Law**:
   - $A \cdot (B + C) = (A \cdot B) + (A \cdot C)$
   - $A + (B \cdot C) = (A + B) \cdot (A + C)$

## Step-by-Step Example

Let's simplify the expression $(\overline{X}Y) + (\overline{Y}Z)$ using Boolean algebra laws:

1. Apply the Distributive Law: 
   
   $(\overline{X}Y) + (\overline{Y}Z) = (\overline{X}+ \overline{Y})(\overline{X}+Z)$

2. Apply the Complement Law: 

    $\overline{\overline{X}}= X$

3. Substitute the complemented variables:

    $(\overline{X}+ Y)(X+Z)$

4. Apply the Idempotent Law:

    $(\overline{X}+ Y)(X+Z)= X(\bar Y)+YZ$

Therefore, the simplified expression is $X(\bar Y)+YZ$.