[[Eigenvalues]]

Eigenvalue is a fundamental concept in [[linear algebra]] that plays a crucial role in understanding the behavior of linear transformations and systems of linear equations. It is a scalar value associated with a square matrix that represents the scaling factor of its corresponding eigenvector.

## Definition

Let $A$ be an $n \times n$ square matrix. An **eigenvector** of $A$ is a non-zero vector $\mathbf{v}$ such that when multiplied by $A$, it results in a scalar multiple of itself, denoted by $\lambda$. This scalar multiple $\lambda$ is called an **eigenvalue** of $A$. In other words, if $\mathbf{v}$ is an eigenvector of $A$, then:

$$ A\mathbf{v} = \lambda \mathbf{v} $$

## Properties

1. Every square matrix has at least one eigenvalue.
2. The number of distinct eigenvalues of a matrix is equal to its dimension.
3. [[Eigenvectors]] corresponding to different eigenvalues are linearly independent.
4. The sum of all eigenvalues of a matrix is equal to its [[trace]], and the product of all eigenvalues is equal to its determinant.

## Finding Eigenvalues and [[Eigenvectors]]

To find the eigenvalues and [[eigenvectors]] of a matrix, we can solve the characteristic equation:

$$ \det(A - \lambda I) = 0 $$

where $I$ is the [[identity matrix]]. The solutions to this equation are the eigenvalues $\lambda_1, \lambda_2, ..., \lambda_n$. To find the corresponding [[eigenvectors]], we substitute each eigenvalue into the equation $A\mathbf{v} = \lambda \mathbf{v}$ and solve for $\mathbf{v}$.

## Diagonalization

If a square matrix has $n$ linearly independent [[eigenvectors]], it can be diagonalized by creating a diagonal matrix $D$ with the eigenvalues on the main diagonal and a matrix $P$ whose columns are the corresponding [[eigenvectors]]. This process is known as **diagonalization** and can be represented as:

$$ A = PDP^{-1} $$

where $D$ is a diagonal matrix with $\lambda_1, \lambda_2, ..., \lambda_n$ on the main diagonal and $P$ is an invertible matrix with $\mathbf{v}_1, \mathbf{v}_2, ..., \mathbf{v}_n$ as its columns.

## Applications

Eigenvalues and [[eigenvectors]] have various applications in mathematics, physics, engineering, and computer science. Some of these include:

- Solving systems of differential equations
- Image processing and compression
- Principal component analysis (PCA) in data analysis
- Markov chains in probability theory
- Quantum mechanics in physics

## Theorems

1. **Cayley-Hamilton Theorem:** Every square matrix satisfies its own characteristic equation.
2. **Spectral Theorem:** A symmetric matrix has real eigenvalues and orthogonal [[eigenvectors]].
3. **Perron-Frobenius Theorem:** For a non-negative square matrix with at least one positive entry, the largest eigenvalue is real and dominant.

## Example

Consider the following $2 \times 2$ matrix:

$$ A = \begin{bmatrix} 3 & -4 \\ 2 & -1 \end{bmatrix} $$

To find its eigenvalues, we solve the characteristic equation:

$$ \det(A - \lambda I) = (3-\lambda)(-1-\lambda) + 8 = 0 $$

which gives us eigenvalues $\lambda_1 = 4$ and $\lambda_2 = -2$. To find the corresponding [[eigenvectors]], we substitute each eigenvalue into the equation $A\mathbf{v} = \lambda \mathbf{v}$ and solve for $\mathbf{v}$. This gives us the [[eigenvectors]] $\mathbf{v}_1 = [1, 1]^T$ and $\mathbf{v}_2 = [2, -1]^T$.

To diagonalize $A$, we create a diagonal matrix $D$ with the eigenvalues on the main diagonal:

$$ D = \begin{bmatrix} 4 & 0 \\ 0 & -2 \end{bmatrix} $$

and a matrix $P$ with the [[eigenvectors]] as its columns:

$$ P = \begin{bmatrix} 1 & 2 \\ 1 & -1 \end{bmatrix} $$

Therefore, we can write:

$$ A = PDP^{-1} = \begin{bmatrix} 1 & 2 \\ 1 & -1 \end{bmatrix} \begin{bmatrix} 4 & 0 \\ 0 & -2 \end{bmatrix} \begin{bmatrix}\frac{-1}{3} & -\frac{2}{3}\\-\frac{-4}{3}&\frac{-5}{3}\end{bmatrix}= 
\begin{bmatrix}\frac{-5}{3}&\frac{-8}{3}\\-\frac{-4}{3}&\frac{-7}{3}\end{bmatrix}
$$

This shows that $A$ is diagonalizable and its eigenvalues and [[eigenvectors]] can be used to simplify its calculations.