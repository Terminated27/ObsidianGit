#prog 

The simplex method is a widely used algorithm for solving linear programming problems. It was developed by George Dantzig in 1947 and has since become one of the most important tools in optimization.

## Problem Formulation

A linear programming problem can be formulated as follows:

**Minimize:** $c^Tx$

**Subject to:** $Ax \geq b$

**Where:**

- $x$ is a vector of decision variables.
- $c$ is a vector of coefficients representing the objective function.
- $A$ is a matrix representing the constraints.
- $b$ is a vector of constants representing the right-hand side of the constraints.

## Basic Feasible Solution (BFS)

A basic feasible solution (BFS) is an assignment of values to the decision variables that satisfies all the constraints. In other words, it is a feasible solution that also satisfies the requirement that at most $m$ variables are nonzero, where $m$ is the number of constraints.

## Simplex Tableau

The simplex method operates on a tableau, which is an augmented matrix that represents the linear programming problem. The tableau consists of two parts: the objective row and the constraint rows.

The objective row contains coefficients for each decision variable and an additional column for the constant term. The constraint rows contain coefficients for each variable, along with an additional column for the right-hand side constant.

## Pivot Operation

The pivot operation is used to move from one BFS to another BFS with improved objective value. It involves selecting a pivot element and performing row operations to make it equal to 1, while making all other elements in its column equal to 0.

## Optimality Test

To determine if a given BFS is optimal, we examine the coefficients in the objective row. If all coefficients are non-negative, then we have reached an optimal solution. Otherwise, we select a negative coefficient as our pivot column and proceed with the pivot operation.

## Simplex Algorithm

The simplex algorithm can be summarized as follows:

1. Start with an initial BFS.
2. Perform the optimality test. If the current BFS is optimal, stop.
3. Select a pivot column with a negative coefficient in the objective row.
4. Choose a pivot row using the minimum ratio test.
5. Perform the pivot operation to obtain a new BFS.
6. Repeat steps 2-5 until an optimal solution is reached.

## Key Theorems

### Fundamental Theorem of Linear Programming

The fundamental theorem of linear programming states that if a linear programming problem has an optimal solution, then it must occur at one of the extreme points (BFS) of the feasible region.

### Optimality Condition

If an optimal solution exists, then at least one of the non-basic variables will have a coefficient of 0 in the objective row.

## Example

Consider the following linear programming problem:

**Minimize:** $z = 3x_1 + 2x_2$

**Subject to:**

$2x_1 + x_2 \geq 4$

$x_1 + 2x_2 \geq 3$

$x_1, x_2 \geq 0$

We can represent this problem in tableau form as follows:

$$
\begin{array}{cccc|c}
-3 & -2 & 0 & 0 & 0 \\
\hline
2 & 1 & -1 & 0 & -4 \\
1 & 2 & 0 & -1 & -3 \\
\end{array}
$$

Starting with an initial BFS at $(x_3, x_4) = (4, 3)$, we perform row operations to obtain a new BFS:

$$
\begin{array}{cccc|c}
-7 & 0 & -2 & 3 & -12 \\
\hline
1 & 0.5 & -0.5 & 0 & -2 \\
-1.5 & 1.5 & 0.5 & -1 & -4.5 \\
\end{array}
$$

Continuing this process, we eventually reach an optimal solution at $(x_1, x_2) = (1, 2)$ with $z = 7$.

## Conclusion

The simplex method provides an efficient algorithm for solving linear programming problems. By iteratively improving the objective value through pivot operations, it converges to the optimal solution. Understanding the simplex method and its key theorems is crucial for tackling optimization problems in various fields of study and industry applications.