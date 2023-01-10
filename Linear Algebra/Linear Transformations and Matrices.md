Transformation = function. However, in linear algebra we use transformation because it's like moving a vector.

# Linear Transformation

Linear transformation = transformation that keeps grid of space straight and origin constant. 

Constants for vector's components in linear combination of basis vectors -> remains the same for linearly transformed basis vectors.

All of this means that all you need is 4 numbers to represent linear transformation: the terminal point of $\hat{i}$ and the terminal point of $\hat{j}$ after the transformation. Given that $\hat{i}$ lands at $(a,b)$ and $\hat{j}$ lands at $(c,d)$, you can then package the transformation into a 2x2 matrix: 

$$
\begin{align}
\begin{bmatrix}
a & c \\
b & d
\end{bmatrix}
\end{align}
$$

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

This explains rotation matrices, which are applied in physics and whatnot. 

You can use the inverse of a matrix to find the reversing transformation.