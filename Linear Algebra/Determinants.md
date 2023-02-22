One good way of measuring [[Linear Transformations|linear transformations]] is with how the area of a given region changes. You can think of the determinant of a matrix as a measure of the linear transformation the matrix represents.

When a linear transformation is applied to the space, every region in the space changes area by the same factor, called the **determinant**. For example, if a transformation increases every area by 3, its determinant 3

If a [[Linear Transformations|linear transformation]] transforms the area of a region into 0, then the determinant must be 0. This is a special case and has applications, such as when calculating [[Eigenvectors and Eigenvalues|eigenvectors and eigenvalues]]. We can visualize this linear transformation as squishing a grid into a lower dimension

If the orientation of space is inverted, then determinant is negative. You can use RH/LH rule to verify change in orientation.

Above properties are for 2-D but apply to 3D as well. 

# Calculation

The determinant is calculated as follows for a transformation:

$$
\det \left( \begin{bmatrix}
a & b \\
c & d
\end{bmatrix} \right)
= ad - bc
$$

For larger matrices, we use

## Laplace's Expansion

Calculate $\det(A)$

$$
A = \begin{pmatrix}
2 & 0 & 0 & 1 & 3 \\
0 & 4 & 0 & 5 & 0 \\
1 & 0 & -1 & 0 & 0 \\
0 & 0 & 0 & 2 & 1 \\
4 & 1 & 0 & 0 & -2
\end{pmatrix}
$$

$$
\begin{align}
\det(A) &= 1 \cdot \det(\begin{pmatrix}
0 & 0 & 1 & 3 \\
4 & 0 & 5 & 0 \\
0 & 0 & 2 & 1 \\
1 & 0 & 0 & -2
\end{pmatrix}) -1\cdot \det(\begin{pmatrix}
2 & 0 & 1 & 3 \\
0 & 4 & 5 & 0 \\
0 & 0 & 2 & 1 \\
4 & 1 & 0 & -2
\end{pmatrix}) \\
&= 0 - 2\det \begin{pmatrix}
2 & 0 & 3 \\
0 & 4 & 0 \\
4 & 1 & -2
\end{pmatrix} + \det \begin{pmatrix}
2 & 0 & 1 \\
0 & 4 & 5 \\
4 & 1 & 0
\end{pmatrix} \\
&= -2 \cdot 4\det \begin{pmatrix}
2 & 3 \\
4 & -2
\end{pmatrix} + 2\det \begin{pmatrix}
4 & 5 \\
1 & 0
\end{pmatrix} + \det \begin{pmatrix}
0 & 4 \\
4 & 1
\end{pmatrix} \\
&= 128 -10+-16 \\
&= 102
\end{align}
$$

Or you can calculate the same using the 

## Triangle Method

$$
A \to \begin{pmatrix}
2 & 0 & 0 & 1 & 3 \\
0 & 4 & 0 & 5 & 0 \\
0 & 0 & -1 & -\frac{1}{2} & -\frac{3}{2} \\
0 & 0 & 0 & 2 & 1 \\
0 & 0 & 0 & 0 & -\frac{51}{8}
\end{pmatrix}
$$