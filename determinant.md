#math #linearAlg

The determinant is a mathematical function that is defined for square matrices. It is denoted by the symbol $\det(A)$, where $A$ is a square matrix. The determinant provides important information about the matrix, such as whether it is invertible and the scaling factor of linear transformations.

## Definition

For a square matrix $A = [a_{ij}]_{n \times n}$, the determinant is defined as:

$$\det(A) = \sum_{\sigma \in S_n} (-1)^{\text{sgn}(\sigma)} a_{1\sigma(1)} a_{2\sigma(2)} \dotsm a_{n\sigma(n)},$$

where $\sigma$ denotes a permutation of the [[set]] $\{1, 2, \dotsc, n\}$ and $S_n$ represents the [[set]] of all permutations of $n$ elements. The function $\text{sgn}(\sigma)$ is equal to $+1$ if $\sigma$ can be obtained by an even number of transpositions and $-1$ if it can be obtained by an odd number of transpositions.

## Properties

The determinant has several important properties:

1. Multiplicative property: For matrices $A$ and $B$, $\det(AB) = \det(A) \cdot \det(B)$.
2. Scaling property: If we multiply a single row or column of a matrix by a scalar $k$, then the determinant gets multiplied by that scalar: $$\det(kA) = k^n \cdot \det(A),$$
   where $n$ is the [[order]] of the matrix.
3. Transposition property: The determinant remains unchanged when we take transpose of a matrix: $$\det(A^T) = \det(A).$$
4. Inverse property: A square matrix $A$ is invertible if and only if $\det(A) \neq 0$. Moreover, if $A$ is invertible, then the inverse of $A$ can be expressed as: $$A^{-1} = \frac{1}{\det(A)} \operatorname{adj}(A),$$
   where $\operatorname{adj}(A)$ denotes the adjugate matrix of $A$.

## Examples

Let's consider a few examples to illustrate the use of determinants.

**Example 1:** Find the determinant of the matrix $A = \begin{bmatrix} 2 & 3 \\ 4 & -1 \end{bmatrix}$.

Using the definition of determinant, we have:
sgn = [[Sign Function]]

$$\det(A) = (-1)^{\text{sgn}(12)}(2)(-1) + (-1)^{\text{sgn}(21)}(3)(4) = -2 -12 = -14.$$

Therefore, $\det(A) = -14$.

**Example 2:** Determine if the matrix $B = \begin{bmatrix} 3 & 1 & 5 \\ 2 & -2 & 7 \\ -1 & 6 & -4 \end{bmatrix}$ is invertible.

To check if $B$ is invertible, we need to calculate its determinant:

$$\det(B) = (-1)^{\text{sgn}(123)}(3)(-2)(-4) + (-1)^{\text{sgn}(213)}(1)(7)(-1) + (-1)^{\text{sgn}(321)}(5)(2)(6).$$

Evaluating this expression, we find that $\det(B) = -8 + 7 +60 =59$. Since $\det(B)\neq0$, we conclude that $B$ is invertible.

## Theorems

There are several important theorems related to determinants:

**Theorem 1:** If a square matrix $A$ has a row or column consisting entirely of zeros, then $\det(A) = 0$.

**Theorem 2:** If two rows or columns of a square matrix $A$ are interchanged to obtain matrix $B$, then $\det(B) = -\det(A)$.

**Theorem 3 (Cramer's Rule):** Consider a system of [[linear]] equations $AX = B$, where $A$ is an invertible matrix. The [[unique]] solution for this system can be expressed as $$X_i = \frac{\det(B_i)}{\det(A)},$$ where $X_i$ denotes the $i$-th component of the solution vector $X$, and $B_i$ is obtained by replacing the $i$-th column of $A$ with the column vector $B$.

**Theorem 4:** If a square matrix $A$ is upper triangular or lower triangular, then the determinant of $A$ is equal to the product of its diagonal elements. In other words, if $A$ is an upper triangular matrix with diagonal entries $a_{ii}$, then $\det(A) = a_{11} \cdot a_{22} \cdot \ldots \cdot a_{nn}$.

**Theorem 5:** If two rows or columns of a square matrix $A$ are proportional, then $\det(A) = 0$. In other words, if the entries in one row (or column) of $A$ can be obtained by multiplying the corresponding entries in another row (or column) by a scalar, then the determinant of $A$ is zero.

**Theorem 6:** If two rows or columns of a square matrix $A$ are identical, then $\det(A) = 0$. In other words, if all the entries in one row (or column) of $A$ are equal to the corresponding entries in another row (or column), then the determinant of $A$ is zero.

**Theorem 7:** If matrix $B$ is obtained from [[matrix]] $A$ by adding a multiple of one row (or column) to another row (or column), then $\det(B) = \det(A)$. In other words, performing an elementary row operation or elementary column operation does not change the determinant.