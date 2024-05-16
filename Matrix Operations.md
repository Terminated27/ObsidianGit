#linearAlg #math 

In [[linear algebra]], [[matrix]] operations are fundamental operations performed on matrices. Matrices are rectangular arrays of numbers, symbols, or expressions arranged in rows and columns. In this atomic note, we will explore various [[matrix]] operations and their properties.

## Matrix Addition

Matrix addition is performed by adding corresponding elements of two matrices of the same size. Let's consider two matrices A and B:

$$
A = \begin{bmatrix} a_{11} & a_{12} \\ a_{21} & a_{22} \end{bmatrix}, \quad
B = \begin{bmatrix} b_{11} & b_{12} \\ b_{21} & b_{22} \end{bmatrix}
$$

The sum of matrices A and B, denoted as A + B, is obtained by adding corresponding elements:

$$
A + B = \begin{bmatrix} a_{11} + b_{11} & a_{12} + b_{12}\\ a_{21} + b_{21}& a_{22} + b_{22}\end{bmatrix}
$$

[[Matrix]] addition is commutative, meaning that A + B = B + A.

## [[Matrix]] Subtraction

[[Matrix]] subtraction is performed by subtracting corresponding elements of two matrices of the same size. Using the same matrices A and B as before, the difference between A and B, denoted as A - B, is obtained by subtracting corresponding elements:

$$
A - B = \begin{bmatrix} a_{11}-b_{11}&a_{12}-b_{12}\\a_{21}-b_{21}&a_ {22}-b_ {22}\end{bmatrix}
$$

## Scalar Multiplication

Scalar multiplication involves multiplying each element of a [[matrix]] by a scalar (a single number). Let's consider the [[matrix]] A:

$$
A = \begin{bmatrix} a_{11} & a_{12} \\ a_{21} & a_{22} \end{bmatrix}
$$

The scalar multiplication of [[matrix]] A by a scalar c, denoted as cA, is obtained by multiplying each element of A by c:

$$
cA = \begin{bmatrix} ca_{11} & ca_{12}\\ ca_{21}& ca_{22}\end{bmatrix}
$$

## Matrix Multiplication

[[Matrix]] multiplication is a binary operation that combines two matrices to produce another matrix. Let's consider two matrices A and B:

$$
A = \begin{bmatrix} a_{11} & a_{12}\\a_{21}&a_{22}\end{bmatrix}, \quad
B = \begin{bmatrix} b_{11}& b_ {12}\\ b_ {21}& b_ {22}\end{bmatrix}
$$

The product of matrices A and B, denoted as AB, is obtained by multiplying the rows of A with the columns of B:

$$
AB = \begin{bmatrix} a_ {11} b_ {11} + a_ {12} b_ {21}&a_ {11} b_ {12} + a_ {12} b_ {22}\\a_ {21} b_ {11 }+a _{22 }b _{21 }&a _{21 }b _{12 }+a _{22 }b _{22 }\end{bmatrix}
$$

[[Matrix]] multiplication is not commutative in general, meaning that AB ≠ BA. However, it is associative, which means that (AB)C = A(BC).

## [[Identity Matrix]]

The [[identity matrix]], denoted as I or I<sub>n</sub>, is a square matrix with ones on the main diagonal and zeros elsewhere. Let's consider the 2x2 [[identity matrix]]:

$$
I = \begin{bmatrix} 1 & 0 \\ 0 & 1 \end{bmatrix}
$$

For any matrix A of appropriate size, the product of A and the [[identity matrix]] is equal to A itself:

$$
AI = IA = A
$$

## [[Inverse Matrix]]
#math #linearAlg 

The inverse of a square matrix A, denoted as A<sup>-1</sup>, is a matrix that, when multiplied by A, gives the [[identity matrix]] I:

$$
AA^{-1} = A^{-1}A = I
$$

Not all matrices have inverses. If a matrix has an inverse, it is said to be invertible or non-singular.

## Transpose of a Matrix

The transpose of a matrix A, denoted as A<sup>T</sup>, is obtained by interchanging its rows and columns. Let's consider the matrix A:

$$
A = \begin{bmatrix} a_{11} & a_{12}\\a_{21}&a_{22}\end{bmatrix}
$$

The transpose of A is given by:

$$
A^T = \begin{bmatrix} a_{11} & a_{21}\\a_{12}&a_{22}\end{bmatrix}
$$
## Matrix Conjugation

Matrix conjugation involves taking the conjugate of each element in a complex matrix A. If:

$$
A = [a_{ij}] \quad \text{where } a_{ij} \text{ is a complex number}
$$

The conjugate of A, denoted as A<sup>*</sup>, is obtained by replacing each element with its [[complex conjugate]]:

$$
A^* = [a_{ij}^*] \quad 
$$
where $a_{ij}^*$ is the [[complex conjugate]] of  $a_{ij}$

For example, if:

$$
A = \begin{bmatrix} 2 + 3i & 1 - 2i \\ 4 & -i \end{bmatrix}
$$

Then the conjugate of A is:

$$
A^* = \begin{bmatrix} 2 - 3i & 1 + 2i \\ 4 & i \end{bmatrix}
$$
## Conclusion

Matrix operations are fundamental in [[linear algebra]] and play a crucial role in various applications such as solving systems of linear equations, representing transformations, and analyzing networks. Understanding these operations and their properties is essential for further exploration in this field.