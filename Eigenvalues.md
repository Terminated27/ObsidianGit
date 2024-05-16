#linearAlg #math  
[[Eigenvalue]]
## Definition
In [[linear algebra]], eigenvalues are a fundamental concept that arises when studying linear transformations. 

**Definition:** Let $A$ be an $n \times n$ matrix. A scalar $\lambda$ is called an [[Eigenvalue]] of $A$ if there exists a non-zero vector $\mathbf{v}$ such that $A\mathbf{v} = \lambda\mathbf{v}$. The vector $\mathbf{v}$ is called an eigenvector corresponding to the [[Eigenvalue]] $\lambda$.

## Finding Eigenvalues
To find the eigenvalues of a matrix, we need to solve the [[characteristic equation]].

**Theorem:** Let $A$ be an $n \times n$ matrix. The eigenvalues of $A$ are the solutions to the [[characteristic equation]] $\det(A - \lambda I) = 0$, where $I$ is the [[identity matrix]] of size $n \times n$. 

To find the eigenvalues, we set up and solve this equation.

### Example:
Consider the matrix 
$$
A = \begin{bmatrix}
2 & 1 \\
1 & 3 \\
\end{bmatrix}
$$

We want to find its eigenvalues.

The [[characteristic equation]] is given by:
$$
\det(A - \lambda I) = 0
$$

Substituting in the values of $A$ and $I$, we have:
$$
\begin{vmatrix}
2 - \lambda & 1 \\
1 & 3 - \lambda \\
\end{vmatrix} = 0
$$

Expanding this [[determinant]], we get:
$$
(2-\lambda)(3-\lambda) - (1)(1) = 0
$$

Simplifying further, we have:
$$
6 - 5\lambda + \lambda^2 - 1 = 0
$$

Rearranging the terms, we obtain a quadratic equation:
$$
\lambda^2 - 5\lambda + 5 = 0
$$

Solving this quadratic equation, we find the eigenvalues:
$$
\lambda_1 = \frac{5 + \sqrt{5}}{2} \quad \text{and} \quad \lambda_2 = \frac{5 - \sqrt{5}}{2}
$$

Therefore, the eigenvalues of matrix $A$ are $\frac{5 + \sqrt{5}}{2}$ and $\frac{5 - \sqrt{5}}{2}$.

## Properties of Eigenvalues
Eigenvalues possess several important properties that are useful in various applications.

1. The sum of eigenvalues of a matrix is equal to the [[trace]] of the matrix. 

   **Theorem:** Let $A$ be an $n \times n$ matrix with eigenvalues $\lambda_1, \lambda_2, ..., \lambda_n$. Then,
   $$
   \sum_{i=1}^{n}\lambda_i = \text{trace}(A)
   $$

2. The product of eigenvalues of a matrix is equal to its [[determinant]].

   **Theorem:** Let $A$ be an $n\times n$ matrix with eigenvalues $\lambda_1, \lambda_2, ..., \lambda_n$. Then,
   $$
   \prod_{i=1}^{n}\lambda_i = |A|
   $$

3. If all eigenvalues of a square matrix $A$ are non-zero, then the inverse of $A$ exists.

   **Theorem:** Let $A$ be an invertible square matrix with eigenvalues $\lambda_1, \lambda_2, ..., \lambda_n$. If none of the eigenvalues are zero, then $A$ is invertible and its inverse is given by
   $$
   A^{-1} = \frac{1}{\lambda_1}\mathbf{v}_1\mathbf{v}_1^T + \frac{1}{\lambda_2}\mathbf{v}_2\mathbf{v}_2^T + ... + \frac{1}{\lambda_n}\mathbf{v}_n\mathbf{v}_n^T
   $$
   where $\mathbf{v}_i$ is the eigenvector corresponding to [[Eigenvalue]] $\lambda_i$.

These properties provide valuable insights into the behavior and characteristics of matrices based on their eigenvalues.

## Conclusion
Eigenvalues play a crucial role in [[linear algebra]], providing information about the behavior of linear transformations represented by matrices. They can be found by solving the [[characteristic equation]] and possess important properties related to the [[trace]], [[determinant]], and invertibility of matrices. Understanding eigenvalues enhances our understanding of linear transformations and enables us to solve various problems in mathematics and other fields.

