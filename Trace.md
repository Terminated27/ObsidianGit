#linearAlg #math 

The trace of a [[square matrix]] $A$, denoted as $\text{tr}(A)$, is the sum of the elements on its main diagonal. In other words, it is the sum of all the entries $a_{ii}$ where $1 \leq i \leq n$, and $n$ is the dimension of the matrix.

## Properties of Trace

1. **Linearity**: For any scalar $\alpha$ and matrices $A$ and $B$ of appropriate dimensions,
$$\text{tr}(\alpha A) = \alpha \cdot \text{tr}(A)$$
$$\text{tr}(A + B) = \text{tr}(A) + \text{tr}(B)$$

2. **Cyclic Property**: For any square matrices $A$ and $B$ such that their product $AB$ is defined,
$$\text{tr}(AB) = \text{tr}(BA)$$

3. **Trace of [[Transpose]]**: For any square matrix $A$,
$$\text{tr}(A^T) = \text{tr}(A)$$

4. **Trace of Similar Matrices**: If two matrices $A$ and $B$ are similar, i.e., there exists an invertible matrix $P$ such that $B = P^{-1}AP$, then they have the same trace:
$$\text{tr}(A) = \text{tr}(B)$$

## Examples:

**Example 1:** Let's calculate the trace of a matrix:
Consider the matrix
$$ A = 
\begin{bmatrix}
    3 & 2 \\
    -1 & 4 \\
\end{bmatrix}
$$
The trace of this matrix is given by
$$\text{tr}(A) = 3 + 4 = 7$$

**Example 2:** Trace of a product of matrices:
Consider the matrices
$$ A = 
\begin{bmatrix}
    1 & 2 \\
    -1 & 3 \\
\end{bmatrix}
\quad \text{and} \quad
B = 
\begin{bmatrix}
    5 & -1 \\
    2 & 4 \\
\end{bmatrix}
$$
We can calculate the product $AB$ as follows:
$$ AB = 
\begin{bmatrix}
    (1 \cdot 5) + (2 \cdot 2) & (1 \cdot -1) + (2 \cdot 4) \\
    (-1 \cdot 5) + (3 \cdot 2) & (-1 \cdot -1) + (3 \cdot 4) \\
\end{bmatrix}
= 
\begin{bmatrix}
    9 & 7 \\
    7 & 13 \\
\end{bmatrix}
$$
Now, let's calculate the trace of $AB$ and $BA$:
$$\text{tr}(AB) = (9 + 13) =22$$
$$\text{tr}(BA) = (5 +12)=17$$
As we can see, $\text{tr}(AB)$ is equal to $\text{tr}(BA)$, which demonstrates the cyclic property of trace.

These properties and examples provide insights into the behavior and applications of trace in [[linear algebra]].