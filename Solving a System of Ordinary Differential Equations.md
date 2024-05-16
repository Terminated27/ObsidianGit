#math #diffeq 

In this atomic note, we will explore the topic of solving a [[system of ordinary differential equations]] (ODEs). We will discuss key theorems, definitions, and step-by-step examples to gain a deeper understanding of this topic.

## Introduction

A [[system of ordinary differential equations]] is a [[set]] of equations that describe how multiple variables change with respect to an independent variable. It is often represented in matrix form as:

$$\frac{d\mathbf{y}}{dt} = \mathbf{f}(t, \mathbf{y})$$

where $\mathbf{y}$ is a vector representing the dependent variables, $t$ is the independent variable (usually time), and $\mathbf{f}(t, \mathbf{y})$ is a vector-valued function that defines the rates of change for each variable.

## [[Existence and Uniqueness Theorem]]

Before we dive into solving systems of ODEs, let's discuss the [[existence and uniqueness theorem]]. This theorem ensures that under certain conditions, there exists a unique solution to an initial value problem for a system of ODEs.

**Theorem:** Suppose $\mathbf{f}(t,\mathbf{y})$ is continuous in both $t$ and $\mathbf{y}$ on some open rectangle $R: a < t < b$, $c < y_1 < d$, $c < y_2 < d$, ..., $c < y_n < d$. Then for any point $(t_0,\mathbf{y}_0)$ in $R$, there exists an interval $I$ containing $t_0$ such that there exists a unique solution $\mathbf{\phi}(t)$ defined on $I$ to the initial value problem:

$$\frac{d\mathbf{y}}{dt} = \mathbf{f}(t, \mathbf{y}), \quad \mathbf{y}(t_0) = \mathbf{y}_0$$

## Solving Systems of ODEs

To solve a system of ODEs, we can use various methods such as the matrix exponential method, the [[Eigenvalue]]-eigenvector method, or numerical methods like Euler's method or Runge-Kutta methods. Here, we will focus on the matrix exponential method.

### Matrix Exponential Method

The matrix exponential method is based on the fact that the solution to a linear homogeneous system of ODEs can be written as:

$$\mathbf{y}(t) = e^{At}\mathbf{c}$$

where $A$ is a constant coefficient matrix and $\mathbf{c}$ is a vector of constants determined by initial conditions.

To solve a non-homogeneous system of ODEs, we can use the variation of parameters technique. The [[general solution]] can be written as:

$$\mathbf{y}(t) = e^{At}\int e^{-At}\mathbf{f}(t)\ dt + e^{At}\mathbf{c}$$

where $\int e^{-At}\mathbf{f}(t)\ dt$ represents the [[integral]] of $\mathbf{f}(t)$ with respect to $t$.

### Example

Let's consider the following system of ODEs:

$$\frac{dx}{dt} = 2x + y$$
$$\frac{dy}{dt} = -x + 3y$$

We can write this system in matrix form as:

$$\frac{d\mathbf{x}}{dt} = \begin{bmatrix} 2 & 1 \\ -1 & 3 \end{bmatrix} \mathbf{x}$$

where $\mathbf{x} = \begin{bmatrix} x \\ y \end{bmatrix}$.

To solve this system using the matrix exponential method, we need to find the matrix $A$ and its exponential $e^{At}$. In this case, $A = \begin{bmatrix} 2 & 1 \\ -1 & 3 \end{bmatrix}$.

Next, we calculate the eigenvalues and [[eigenvectors]] of $A$. Let $\lambda_1$ and $\lambda_2$ be the eigenvalues and $\mathbf{v}_1$ and $\mathbf{v}_2$ be the corresponding [[eigenvectors]]. Then we have:

$$\lambda_1 = 2, \quad \mathbf{v}_1 = \begin{bmatrix} 1 \\ -1 \end{bmatrix}$$
$$\lambda_2 = 4, \quad \mathbf{v}_2 = \begin{bmatrix} 1 \\ 1 \end{bmatrix}$$

Now, we can write the solution as:

$$\mathbf{x}(t) = e^{At}\mathbf{c} = c_1e^{2t}\begin{bmatrix} 1 \\ -1 \end{bmatrix} + c_2e^{4t}\begin{bmatrix} 1 \\ 1 \end{bmatrix}$$

where $c_1$ and $c_2$ are constants determined by initial conditions.

## Conclusion

Solving a [[system of ordinary differential equations]] involves finding a unique solution that satisfies the given initial conditions. The matrix exponential method provides an elegant way to solve linear homogeneous systems of ODEs, while the variation of parameters technique can be used for non-homogeneous systems. Understanding these methods and applying them to specific examples allows us to analyze and predict the behavior of complex systems described by ODEs. 