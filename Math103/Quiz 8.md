Given Matrix A

$$
A = \begin{bmatrix}
3 & 6 & 9 \\
2 & 5 & 1 \\
1 & 1 & 8
\end{bmatrix}
$$

# Part 1

1. Find E1 such that
$$
E_{1} \cdot A = \begin{bmatrix}
1 & 2 & 3 \\
2 & 5 & 1 \\
1 & 1 & 8
\end{bmatrix}
$$

$$
E_{1} = \begin{bmatrix}
\frac{1}{3} & 0 & 0 \\
0 & 1 & 0 \\
0 & 0 & 1
\end{bmatrix}
$$

2. Find $E_{2}$ such that 

$$
E_{2} \cdot \begin{bmatrix}
1 & 2 & 3 \\
2 & 5 & 1 \\
1 & 1 & 8
\end{bmatrix} = \begin{bmatrix}
1 & 2 & 3 \\
0 & 1 & -5 \\
1 & 1 & 8
\end{bmatrix}
$$

$$
E_{2} = \begin{bmatrix}
1 & 0 & 0 \\
0 & 1 & -1 \\
0 & 0 & 1
\end{bmatrix}
$$

3. Find $E_{3}$ such that 

$$
E_{3} \cdot \begin{bmatrix}
1 & 2 & 3 \\
0 & 1 & -5 \\
1 & 1 & 8
\end{bmatrix} = \begin{bmatrix}
1 & 2 & 3 \\
0 & 1 & -5 \\
0 & -1 & 5
\end{bmatrix}
$$

$$
E_{3} = \begin{bmatrix}
1 & 0 & 0 \\
0 & 1 & 0 \\
-1 & 0 & 1
\end{bmatrix}
$$

4. Find $E_{4}$ such that

$$
E_{4} \cdot \begin{bmatrix}
1 & 2 & 3 \\
0 & 1 & -5 \\
0 & -1 & 5
\end{bmatrix} = \begin{bmatrix}
1 & 2 & 3 \\
0 & 1 & -5 \\
0 & 0 & 0
\end{bmatrix}
$$

$$
E_{4} = \begin{bmatrix}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & 1 & 1
\end{bmatrix}
$$

# Part 2

Find the inverse of each matrix above

$$
\begin{align}
E_{1}^{-1} &= \begin{bmatrix}
3 & 0 & 0 \\
0 & 1 & 0 \\
0 & 0 & 1
\end{bmatrix} \\
E_{2}^{-1} &= \begin{bmatrix}
1 & 0 & 0 \\
0 & 1 & 1 \\
0 & 0 & 1
\end{bmatrix} \\
E_{3} &= \begin{bmatrix}
1 & 0 & 0 \\
0 & 1 & 0 \\
1 & 0 & 1
\end{bmatrix} \\
E_{4} &= \begin{bmatrix}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & -1 & 1
\end{bmatrix}
\end{align}
$$