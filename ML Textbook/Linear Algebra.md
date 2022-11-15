# Matrices, Vectors, Scalars, Tensors

## Scalars
- single number
- lowercase character, like $x$

## Vectors
- array
- points in space
- bold lower case, like $\mathbf{x}$

## Matrices
- 2-D array
- bold uppercase, like $\mathbf{X}$

## Tensors
- 3+ dimensions

## Matrix Operations

### Transposition
- mirror matrix across main diagonal (upper left to bottom right)
- $\mathbf{A}^{\top}_{i, j} = \mathbf{A}_{j, i}$
- For vectors, columns -> rows, rows -> columns

### Addition, Multiplication
- works with same shape, just add element-wise

### Broadcasting
- vector is filled to form a matrix of same size
- implicit when adding vector to matrix of same dimension on one side

# Multiplying Matrices and Vectors

- matrix product is just dot product but with each vector
- element-wise product is different
- distributive
- associative
- NOT commutative for matrices, yes for vectors
- $(AB)^{\top} = B^{\top}A^{\top}$
- system of linear equations: $\mathbf{A}x = b$, where $x = [x_{1}, x_{2}, \dots, x_{n}]$ is a set of variables we are solving for

# Identity and Inverse Matrices
- used to solve for 
