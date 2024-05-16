
#math #diffeq 
A [[linear]] [[system of ordinary differential equations]] (ODEs) is a [[set]] of first-[[order]] ODEs that can be written in [[matrix]] form as:

$$\frac{d\mathbf{x}}{dt} = A\mathbf{x}$$

where $\mathbf{x}$ is a vector function of $t$, and $A$ is a constant coefficient [[matrix]].

## Key Theorems

### [[Existence and Uniqueness Theorem]]
The [[existence and uniqueness theorem]] for [[linear]] systems states that if $A$ is continuous on an [[open interval]] $I$ containing $t_0$, then there exists a unique solution $\mathbf{x}(t)$ defined on $I$ that satisfies the [[initial condition]] $\mathbf{x}(t_0) = \mathbf{x}_0$, where $\mathbf{x}_0$ is a given vector.

### [[Superposition Principle]]
The [[superposition]] principle states that if $\mathbf{x}_1(t)$ and $\mathbf{x}_2(t)$ are solutions to the [[linear system]], then any [[linear combination]] of these solutions, i.e., $c_1\mathbf{x}_1(t) + c_2\mathbf{x}_2(t)$, where $c_1$ and $c_2$ are constants, is also a solution.

## Definitions

### Homogeneous Linear System
A homogeneous linear system of ODEs is obtained when the right-hand side of the equation is zero. It can be written as:

$$\frac{d\mathbf{x}}{dt} = A\mathbf{x}$$

where $\mathbf{x}$ is a vector function of $t$, and $A$ is a constant coefficient matrix.

### Inhomogeneous Linear System
An inhomogeneous linear system of ODEs includes a non-zero term on the right-hand side. It can be written as:

$$\frac{d\mathbf{x}}{dt} = A\mathbf{x} + \mathbf{g}(t)$$

where $\mathbf{x}$ is a vector function of $t$, $A$ is a constant coefficient matrix, and $\mathbf{g}(t)$ is a given vector function.

## Step-by-Step Example

Certainly! Here is the entire solution, combining all the steps:

Consider the following linear [[system of ordinary differential equations]] (ODEs):

$$
\frac{d}{dt}\begin{bmatrix} x_1 \\ x_2 \end{bmatrix} = \begin{bmatrix} 2 & -1 \\ 3 & 4 \end{bmatrix}\begin{bmatrix} x_1 \\ x_2 \end{bmatrix}
$$

To solve this system, we first find the eigenvalues and [[eigenvectors]] of the coefficient matrix $A$. Let's denote the eigenvalues as $\lambda_1$ and $\lambda_2$, and the corresponding [[eigenvectors]] as $\mathbf{v}_1$ and $\mathbf{v}_2$.

**Step 1: Finding the Eigenvalues and [[Eigenvectors]]**

To find the eigenvalues and [[eigenvectors]] of the coefficient matrix $A = \begin{bmatrix} 2 & -1 \\ 3 & 4 \end{bmatrix}$, we solve the characteristic equation:

$$
\det(A - \lambda I) = 0
$$

where $I$ is the [[identity matrix]]. Substituting in the values, we have:

$$
\begin{vmatrix} 2-\lambda & -1 \\ 3 & 4-\lambda \end{vmatrix} = (2-\lambda)(4-\lambda) - (-1)(3) = \lambda^2 - 6\lambda + 11 = 0
$$

Solving this quadratic equation, we find that the eigenvalues are $\lambda_1 = 3 + i$ and $\lambda_2 = 3 - i$.

To find the corresponding [[eigenvectors]], we substitute each [[Eigenvalue]] back into $(A - \lambda I)\mathbf{v} = \mathbf{0}$ and solve for $\mathbf{v}$.

For $\lambda_1 = 3 + i$, we have:

$$
\begin{bmatrix} -1-i & -1 \\ 3 & 1-i \end{bmatrix}\begin{bmatrix} v_{11} \\ v_{12} \end{bmatrix} = \begin{bmatrix}0 \\0\end{bmatrix}
$$

Simplifying this system of equations, we get:

$$
(v_{11}-v_{12})(-1-i) = (v_{11}-v_{12})(1-i) = 0
$$

This implies that $v_{11} = v_{12}$, so we can choose $v_{11} = 1$ and $v_{12} = 1$. Therefore, the eigenvector corresponding to $\lambda_1$ is $\mathbf{v}_1 = \begin{bmatrix} 1 \\ 1 \end{bmatrix}$.

Similarly, for $\lambda_2 = 3 - i$, we have:

$$
\begin{bmatrix} -1+i & -1 \\ 3 & 1+i \end{bmatrix}\begin{bmatrix} v_{21} \\ v_{22} \end{bmatrix} = \begin{bmatrix}0 \\0\end{bmatrix}
$$

Simplifying this system of equations, we get:

$$
(v_{21}-v_{22})(-1+i) = (v_{21}-v_{22})(1+i) = 0
$$

This implies that $v_{21} = v_{22}$, so we can choose $v_{21} = 1$ and $v_{22} = 1$. Therefore, the eigenvector corresponding to $\lambda_2$ is $\mathbf{v}_2 = \begin{bmatrix} 1 \\ 1 \end{bmatrix}$.

**Step 2: Expressing the [[General Solution]]**

Now that we have the eigenvalues and [[eigenvectors]], we can express the [[general solution]] as:

$$
\mathbf{x}(t) = c_1e^{\lambda_1 t}\mathbf{v}_1 + c_2e^{\lambda_2 t}\mathbf{v}_2
$$

where $c_1$ and $c_2$ are constants determined by initial conditions.

Substituting in the given values of $\lambda_1$, $\lambda_2$, $\mathbf{v}_1$, and $\mathbf{v}_2$, we have:

$$
\mathbf{x}(t) = c_1e^{(3+i)t}\begin{bmatrix} 1 \\ 1 \end{bmatrix} + c_2e^{(3-i)t}\begin{bmatrix} 1 \\ 1 \end{bmatrix}
$$

**Step 3: Solving for the Constants**

To determine the values of $c_1$ and $c_2$, we need to consider the initial conditions. Let's say that at $t = 0$, $\mathbf{x}(0) = \begin{bmatrix} x_{10} \\ x_{20} \end{bmatrix}$.

Substituting this into the [[general solution]], we get:

$$
\mathbf{x}(0) = c_1e^{(3+i)(0)}\begin{bmatrix} 1 \\ 1 \end{bmatrix} + c_2e^{(3-i)(0)}\begin{bmatrix} 1 \\ 1 \end{bmatrix} = c_1\begin{bmatrix} 1 \\ 1 \end{bmatrix} + c_2\begin{bmatrix} 1 \\ 1 \end{bmatrix}
$$

Since $\mathbf{x}(0) = \begin{bmatrix} x_{10} \\ x_{20} \end{bmatrix}$, we can equate the components to solve for $c_1$ and $c_2$:

$$
x_{10}\begin{pmatrix}
    c_1\\
    c_2\\
    \end{pmatrix}
    +
    x_{20}\begin {pmatrix}
    c_1\\
    c_2\\
    \end {pmatrix}
    =
    \begin {pmatrix}
    x_{10}\\
    x_{20}\\
    \end {pmatrix}
$$

This gives us the system of equations:

$$
\begin{align*}
c_1 + c_2 &= x_{10} \\
c_1 + c_2 &= x_{20}
\end{align*}
$$

Since these two equations are identical, we only have one independent equation. Let's choose $c_1 + c_2 = x_{10}$.

Solving this equation for $c_1$, we get:

$$
c_1 = x_{10} - c_2
$$

Therefore, the [[general solution]] becomes:

$$
\mathbf{x}(t) = (x_{10} - c_2)e^{(3+i)t}\begin{bmatrix} 1 \\ 1 \end{bmatrix} + c_2e^{(3-i)t}
\begin{bmatrix} 
1 \\ 1 
\end{bmatrix}
$$

**Step 4: Final Solution**

Finally, we can simplify the [[general solution]] by combining like terms. Since $e^{it}$ and $e^{-it}$ are complex conjugates ([[Euler's Formula]]), their sum is twice the real part. Therefore, we have:

$$
\mathbf{x}(t) = (x_{10} - c_2)\left(e^{3t}\cos(t) + ie^{3t}\sin(t)\right)\begin{bmatrix} 1 \\ 1 \end{bmatrix} + c_2\left(e^{3t}\cos(t) - ie^{3t}\sin(t)\right)\begin{bmatrix} 1 \\ 1 \end{bmatrix}
$$

Combine the real and imaginary parts:

$$
\mathbf{x}(t) = x_{10}e^{3t}\begin{bmatrix} \cos(t) \\ \sin(t) \end{bmatrix} + c_2e^{3t}\begin{bmatrix} 1-i \\ 1-i \end{bmatrix}
$$

The final solution for the given linear system of ODEs is:

$$
\mathbf{x}(t) = x_{10}e^{3t}\begin{bmatrix} \cos(t) \\ \sin(t) \end{bmatrix} + c_2e^{3t}\begin{bmatrix} 1-i \\ 1-i \end{bmatrix}
$$


## Conclusion

Linear systems of ordinary differential equations are important mathematical models used to describe various physical phenomena. The [[existence and uniqueness theorem]] guarantees the existence of a unique solution under certain conditions. The [[superposition]] principle allows us to construct new solutions from existing ones. Understanding the concepts of homogeneous and inhomogeneous systems helps in solving different types of linear [[ODE]] systems.