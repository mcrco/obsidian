One good way of measuring [[Linear Transformations|linear transformations]] is with how the area of a given region changes. You can think of the determinant of a matrix as a measure of the linear transformation the matrix represents.

When a linear transformation is applied to the space, every region in the space changes area by the same factor, called the **determinant**. For example, if a transformation increases every area by 3, its determinant 3

If a [[Linear Transformations|linear transformation]] transforms the area of a region into 0, then the determinant must be 0. This is a special case and has applications, such as when calculating [[Eigenvectors and Eigenvalues|eigenvectors and eigenvalues]]. We can visualize this linear transformation as squishing a grid into a lower dimension

If the orientation of space is inverted, then determinant is negative. You can use RH/LH rule to verify change in orientation.

Above properties are for 2-D but apply to 3D as well. 

The determinant is calculated as follows for a transformation:

$$
\det \left( \begin{bmatrix}
a & b \\
c & d
\end{bmatrix} \right)
= ad - bc
$$