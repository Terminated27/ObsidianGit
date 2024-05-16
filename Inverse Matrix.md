#math #linearAlg 

An inverse matrix is a fundamental concept in [[linear algebra]] that plays a crucial role in solving systems of [[linear]] equations and various other mathematical operations. In this atomic note, we will explore the definition of an inverse matrix, its properties, and how to find the inverse of a [[matrix]].

## Definition

Let's consider a square matrix A of size n x n. If there exists another square matrix B of the same size, such that their product AB is equal to the [[identity matrix]] I<sub>n</sub>, then B is called the **inverse** of A. The inverse of A is denoted by A<sup>-1</sup>.

$$
A \cdot A^{-1} = I_n
$$

## Properties

1. If A has an inverse, then the inverse is unique.
2. If A and B are invertible matrices, then their product AB is also invertible, and $$(AB)^{-1} = B^{-1}A^{-1}$$.
3. The inverse of the inverse of a [[matrix]] is the original [[matrix]] itself: $$(A^{-1})^{-1} = A$$.

## Finding the Inverse

To find the inverse of a [[square matrix]] A, we can use various methods such as Gauss-Jordan elimination or elementary row operations. Let's consider an example to understand this process step-by-step.

**Example:**

Let's find the inverse of the following 2x2 [[matrix]]:

$$
A = \begin{bmatrix}
a & b \\
c & d \\
\end{bmatrix}
$$

Step 1: Calculate the [[determinant]] (ad - bc) of [[matrix]] A.

Step 2: If the [[determinant]] is non-zero (i.e., det(A) ≠ 0), then A has an inverse.

Step 3: Swap the positions of a and d and change the signs of b and c.

Step 4: Multiply the resulting [[matrix]] by 1/det(A).

The resulting matrix is the inverse of A.

## Theorems

### Theorem 1: Inverse of a Product

If A and B are invertible matrices, then the product AB is also invertible, and $$(AB)^{-1} = B^{-1}A^{-1}$$.

### Theorem 2: Inverse of a Transpose

If A is an invertible matrix, then its transpose A<sup>T</sup> is also invertible, and $$(A^T)^{-1} = (A^{-1})^T$$.

### Theorem 3: Inverse of a Scalar Multiple

If A is an [[invertible matrix]] and k ≠ 0 is a scalar, then kA is also invertible, and $$(kA)^{-1} = \frac{1}{k}A^{-1}$$.

## Conclusion

Inverse matrices are powerful tools in [[linear algebra]] that allow us to solve systems of [[linear]] equations, compute determinants, find eigenvalues and [[eigenvectors]], and perform various other operations. Understanding the concept of inverse matrices and their properties provides a solid foundation for further exploration in [[linear algebra]].