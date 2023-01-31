A linear/matrix transformation is just a function. However, in linear algebra we use the term transformation because a function is like moving a vector.

A linear transformation is a transformation that keeps grid of space straight and origin constant. 

# Matrix of a Transformation

The constants for vector's components in linear combination of basis vectors remain the same for linearly transformed basis vectors.

All of this means that all you need is 4 numbers to represent linear transformation: the terminal point of $\hat{i}$ and the terminal point of $\hat{j}$ after the transformation. Given that $\hat{i}$ lands at $(a,b)$ and $\hat{j}$ lands at $(c,d)$, you can then package the transformation into a 2x2 matrix: 

$$
\begin{align}
\begin{bmatrix}
a & c \\
b & d
\end{bmatrix}
\end{align}
$$

This matrix is called the **standard matrix**.

To transform any vector $(x,y)$,  you can just compute as follows:

$$
x \cdot \begin{bmatrix}
a \\
b
\end{bmatrix}
+ y \cdot \begin{bmatrix}
c \\
d
\end{bmatrix}
$$

Or in matrix-vector multiplication form:

$$
\begin{bmatrix}
a & c \\
b & d
\end{bmatrix}
\begin{bmatrix}
x \\
y
\end{bmatrix}
$$

A good example of a transformation matrix with its columns as the new basis vectors are rotation matrices.

You can use the inverse of a matrix to find the reversing transformation.

# Example Problems for Linear Transformations

## Problem 1

$$
\mathbf{A} = \begin{pmatrix}
1 & -3 \\
3 & 5 \\
-1 & 7
\end{pmatrix}, \,
\vec{u} = \begin{pmatrix}
2 \\
-1
\end{pmatrix}, \,
\vec{b} = \begin{pmatrix}
3 \\
2 \\
-5
\end{pmatrix}, \,
\begin{pmatrix}
3 \\
2 \\
5
\end{pmatrix}
$$

**Calculate $T(\vec{u}) = \mathbf{A}\vec{u}$ **

$$
\mathbf{A} \cdot \vec{u} = \begin{pmatrix}
5 \\
1 \\
-9
\end{pmatrix}
$$

**Is $\vec{b}$ in the range of $T$? If it is, find its preimage $\vec{x}$.**

$$
\begin{align}
\mathbf{A} \cdot \vec{x} &= \vec{b} \\
\begin{pmatrix}
1 & -3 \\
3 & 5 \\
-1 & 7
\end{pmatrix} \cdot \begin{pmatrix}
x_{1} \\
x_{2}
\end{pmatrix} &= 
\begin{pmatrix}
3 \\
2 \\
-5
\end{pmatrix} \\
\end{align}
$$


$$
\begin{pmatrix}
1 & -3 & 3 \\
3 & 5 & 2 \\
-1 & 7 & -5
\end{pmatrix}
$$

$$
\begin{align}
R_{2} = R_{2} - 3R_{1}, R_{3} \to R_{1} + R_{3} &\implies \begin{pmatrix}
1 & -3 & 3 \\
0 & 14 & -7 \\
0 & 4 & -2
\end{pmatrix}  \\
R_{3} \to R_{3} - \frac{2}{7}R_{2}, R_{1} \to R_{1} + \frac{3}{4} R_{3} &\implies \begin{pmatrix}
1 & 0 & \frac{3}{2} \\
0 & 1 & -\frac{1}{2} \\
0 & 0 & 0
\end{pmatrix}
\end{align}
$$

$$
\vec{x} = \begin{pmatrix}
\frac{3}{2} \\
-\frac{1}{2}
\end{pmatrix}
$$

**Is $\vec{c}$ in the range of $T$, and find the preimage if so.**

$$
\begin{align}
\mathbf{A} \cdot \vec{x} &= \vec{c} \\
\begin{pmatrix}
1 & -3 \\
3 & 5 \\
-1 & 7
\end{pmatrix} \cdot \begin{pmatrix}
x_{1} \\
x_{2}
\end{pmatrix} &= 
\begin{pmatrix}
3 \\
2 \\
5
\end{pmatrix} \\
\end{align}
$$

$$
\begin{pmatrix}
1 & -3 & 3 \\
3 & 5 & 2 \\
-1 & 7 & -5
\end{pmatrix}
$$

These 3 equations contradict one another.

# Example Problems for Matrices

## Problem 1

Find the standard matrix A for the dilation transformation $T(\vec{x}) = 3\vec{x}, \, \vec{x} \in \mathbb{R^{2}}$


$$
\begin{align}
\vec{e}_{1} &= \begin{bmatrix}
3 \\
0
\end{bmatrix} \\
\vec{e}_{2} &= \begin{bmatrix}
0 \\
3
\end{bmatrix} \\
\mathbf{A} &= \begin{bmatrix}
3 & 0 \\
0 & 3
\end{bmatrix} \\
\end{align}
$$

## Problem 2

$T(\vec{x})$ rotates points about the origin with an angle of $\theta = \frac{-3\pi}{2}$. 

$$
\begin{align}
T(\vec{e}_{1}) &= \begin{bmatrix}
0 \\
1
\end{bmatrix} \\
T(\vec{e_{2}}) &= \begin{bmatrix}
-1 \\
0
\end{bmatrix} \\
\mathbf{A} &= \begin{bmatrix}
0 & -1 \\
1 & 0
\end{bmatrix}
\end{align}
$$

## Problem 3

Find the standard matrix for the reflection across the plane x + y + z = 1.

$$
\begin{align}
D &= \frac{|ax + by + cz + d|}{\lvert \lvert \vec{n} \rvert \rvert } \\
e_{i} &\to e_{i} - 2D \cdot \frac{\vec{n}}{\lvert \lvert \vec{n} \rvert \rvert } \\
D_{e_{1}} &= \begin{bmatrix}
1 \\
0 \\
0
\end{bmatrix} - 2() \\
\mathbf{A} &= \begin{bmatrix}

\end{bmatrix}
\end{align}
$$


