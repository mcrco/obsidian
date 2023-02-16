# Definition

A $n\times n$ matrix is invertible if there is an $n\times n$ matrix $\mathbf{C}$  such that $\mathbf{C}\mathbf{A} = \mathbf{I}$ **and** $\mathbf{A}\mathbf{C} = \mathbf{I}$, where $\mathbf{I}$ is a $n\times n$ identity matrix.

# Finding the Inverse

We can use the product of **elementary matrices** to find the inverse of a matrix. Elementary matrices are matrices that can be derived from the identity matrix with one step.

## Example

Find the inverse of $\mathbf{A}$

$$
\begin{align}
A &= \begin{pmatrix}
4 & 0 & 5 \\
0 & 3 & 0 \\
1 & 0 & 4
\end{pmatrix}  \\
E_{1} = \begin{pmatrix}
\frac{1}{4} & 0 & 0 \\
0 & 1 & 0 \\
0 & 0 & 1
\end{pmatrix} \to
A &= \begin{pmatrix}
1 & 0 & \frac{5}{4} \\
0 & 3 & 0 \\
1 & 0 & 4
\end{pmatrix}  \\
E_{2} = \begin{pmatrix}
1 & 0 & 0 \\
0 & \frac{1}{3} & 0 \\
0 & 0 & 1
\end{pmatrix} \to
A &= \begin{pmatrix}
1 & 0 & \frac{5}{4} \\
0 & 1 & 0 \\
1 & 0 & 4
\end{pmatrix}  \\
E_{3} = \begin{pmatrix}
1 & 0 & 0 \\
0 & 1 & 0 \\
-1 & 0 & 1
\end{pmatrix} \to
A &= \begin{pmatrix}
1 & 0 & \frac{5}{4} \\
0 & 1 & 0 \\
0 & 0 & 4
\end{pmatrix}  \\
E_{4} = \begin{pmatrix}
1 & 0 & 0 \\
0 & 1 & 0 \\
-1 & 0 & 1
\end{pmatrix} \to
A &= \begin{pmatrix}
1 & 0 & \frac{5}{4} \\
0 & 1 & 0 \\
0 & 0 & \frac{11}{4}
\end{pmatrix} \\
E_{5} = \begin{pmatrix}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & 0 & \frac{4}{11}
\end{pmatrix} \to A &= \begin{pmatrix}
1 & 0 & \frac{5}{4} \\
0 & 1 & 0 \\
0 & 0 & 1
\end{pmatrix} \\
E_{6} = \begin{pmatrix}
1 & 0 & -\frac{5}{4} \\
0 & 1 & 0 \\
0 & 0 & 1
\end{pmatrix} \to A &= \begin{pmatrix}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & 0 & 1
\end{pmatrix}
\end{align}
$$

# Properties

## Theorem 1

$$
(\mathbf{A}\mathbf{B})^{-1} = \mathbf{B}^{-1} \cdot \mathbf{A}^{-1}
$$


## Theorem 2

Given Theorem 1, we can use an [[Proofs#Proof By Induction|inductive proof]] to show that given that $A_{1}, A_{2}, A_{3} \dots A_{n}$ are invertible matrices,

$$
(A_{1} \cdot A_{2} \cdot A_{3} \dots A_{n}) ^{-1} = A_{n}^{-1} \cdot A_{n - 1}^{-1} \dots A_{1}^{-1}
$$

Base case: n = 2

The theorem literally states this is true

Inductive step: 

Let $A = (A_{1} \cdot A_{2} \dots A_{n})$, $B = A_{n + 1}$

$$
\begin{align}
(A_{1} \cdot A_{2} \dots A_{n+1})^{-1} &= (A \cdot B)^{-1} \\
&= B^{-1} \cdot A^{-1} \\
&= A_{n + 1}^{-1} \cdot A_{n}^{-1} \cdot A_{n - 1}^{-1} \dots A_{1}
\end{align}
$$

$S(n+ 1)$ holds true given $S(n)$ is true.