#math #linearAlg 

In [[linear algebra]], eigenvectors are a fundamental concept that plays a crucial role in understanding linear transformations and matrices. 

## Definition

Let **A** be an *n x n* square matrix. A non-zero vector **v** is called an eigenvector of **A** if there exists a scalar λ such that:

$$
\mathbf{Av} = \lambda\mathbf{v}
$$

The scalar λ is called the [[Eigenvalue]] corresponding to the eigenvector **v**.

## Properties and Theorems

1. Eigenvectors are non-zero vectors: If **v** is an eigenvector of matrix **A**, then **v** must be non-zero.

2. Eigenvalues may be complex numbers: The eigenvalues of a real matrix can be complex numbers.

3. Eigenvalues are roots of the characteristic equation: The eigenvalues of matrix **A** are the solutions to the characteristic equation:

$$
\text{det}(\mathbf{A} - \lambda\mathbf{I}) = 0
$$

where **I** is the [[identity matrix]] of the same size as **A**.

4. Eigenvectors corresponding to distinct eigenvalues are linearly independent: If λ1, λ2, ..., λk are distinct eigenvalues of matrix **A**, and v1, v2, ..., vk are their corresponding eigenvectors, then v1, v2, ..., vk are linearly independent.

5. Diagonalizable matrices: A square matrix **A** is diagonalizable if it has *n* linearly independent eigenvectors.

## Example

Consider the following 2x2 matrix:

$$
\mathbf{A} = \begin{bmatrix}
3 & 1 \\
0 & 2 \\
\end{bmatrix}
$$

To find its eigenvectors and eigenvalues, we start by solving the characteristic equation:

$$
\text{det}(\mathbf{A} - \lambda\mathbf{I}) = \begin{vmatrix}
3-\lambda & 1 \\
0 & 2-\lambda \\
\end{vmatrix} = (3-\lambda)(2-\lambda) = 0
$$

Setting the [[determinant]] equal to zero, we find two eigenvalues:

$$
\begin{align*}
(3-\lambda)(2-\lambda) &= 0 \\
\Rightarrow \lambda_1 &= 3 \\
\Rightarrow \lambda_2 &= 2 \\
\end{align*}
$$

To find the eigenvectors corresponding to each [[Eigenvalue]], we substitute them back into the equation **Av** = λ**v** and solve for **v**.

For λ1 = 3:

$$
(\mathbf{A} - 3\mathbf{I})\mathbf{v}_1 = \begin{bmatrix}
0 & 1 \\
0 & -1 \\
\end{bmatrix}\mathbf{v}_1 = \mathbf{0}
$$

This system of equations gives us v1 = [t, t]ᵀ, where t is a free parameter. Thus, one eigenvector corresponding to λ1 is [t, t]ᵀ.

For λ2 = 2:

$$
(\mathbf{A} - 2\mathbf{I})\mathbf{v}_2 = \begin{bmatrix}
1 & 1 \\
0 & 0 \\
\end{bmatrix}\mathbf{v}_2 = \mathbf{0}
$$

This system of equations gives us v2 = [-s, s]ᵀ, where s is a free parameter. Thus, one eigenvector corresponding to λ2 is [-s, s]ᵀ.

Therefore, the matrix **A** has two linearly independent eigenvectors: [t, t]ᵀ and [-s, s]ᵀ.

## Conclusion

Eigenvectors are essential in understanding the behavior of linear transformations and matrices. They provide valuable insights into the structure and properties of matrices. The properties and theorems associated with eigenvectors allow us to analyze various aspects of [[linear algebra]] more effectively.