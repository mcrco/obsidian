# p.124 #1, 4, 17, 18, 20, 29, 43, 44, 45, 50, 96, 98 

1. 5366280699654138 -> 0
4. 419-6888-7169-444 -> invalid
17. both
18. neither=
20. neither
29. Every output has at most one input. For every number in the codomain in the form $2^{m}3^{n}$, there is at most one tuple of inputs since prime factorizations are unique. For every number in the codomain not in the form, there is no input.
43. $X = \frac{Y - 2}{4}$
44. $X = \log_{3}Y$
45. $X = 2^{\frac{Y}{3}}$
50. $$
\begin{align}
f \circ f &= 4n + 3 \\
g \circ g &= 9n - 4 \\
f \circ g &= 6n - 1 \\
g \circ f &= 6n + 2
\end{align}
$$

96. 101
98. 111

# p. 137 #10, 45, 50, 73, 128, 142 (a, b, c), 146 

10. 5
45. 12
50. 3
73. 15
<<<<<<< HEAD
128. Proving base case:
$$
\begin{align}
z_{0} &= 2 \\
z_{1} &= 9 \\
\end{align}
$$

Proving inductive step:

$$
\begin{align}
z_{n+1} &= 7z_{n}-10z_{n-1} \\
&= 7(2+n)3^{n} - 10(2+n-1)3^{n-1} \\
&= 14(3)^{n} + 7n(3)^{n} - 10(3)^{n-1}-10n(3)^{n-1} \\
&= \frac{14}{3}3^{n+1} +\frac{7}{3}3^{n+1}-\frac{10}{9}3^{n+1}-\frac{10}{9}n3^{n+1} \\
&= 
\end{align}
$$
=======
128. Base Case
$$
\begin{align}
z_{0} &= -1 \\
z_{1} &= -14 \\
z_{2} &= 7(-14) - 10(-1) = 3 \cdot 2^{2} - 4 \cdot 5^{2} = -88
\end{align}
$$
Induction assuming $r_{n}$ is true:
$$
\begin{align}
r_{n+1} &= 7r_{n} - 10r_{n-1} \\
&= 7(3\cdot 2^{n} - 4 \cdot 5 ^{n}) - 10(3\cdot 2 ^{n-1} - 4 \cdot 5 ^{n-1}) \\
&= 21 \cdot 2 ^{n} - 28 \cdot 5^{n} - 15 \cdot 2^{n} + 8 \cdot 5 ^{n} \\
&= 6 \cdot 2 ^{n} - 20\cdot 5^{n} \\
&= 3 \cdot 2^{n+1} - 4 \cdot 5^{n+1}
\end{align}
$$
142. a. $baabcaaba$
b. caababaab
c. baabbaab
146. 0, 1, 01, 10, 00, 11, 000, 001, 010, 011, 100, 101, 110, 111
>>>>>>> origin/main

# p.150 #18, 19, 24 

18. $\{ (4,1), (5,2), (1,1), (2,2), (3,3), (4,4), (5,5) \}$
19. $\{ (1,4), (2,5), (1,1), (2,2), (3,3), (4,4), (5,5) \}$
24. not reflexive, symmetric, not antisymmetric, not transitive, not ordered

# p.156 #1, 5 or 9, 16, 18, 39 

1. equivalent
5. equivalent
16. yes

# p. 164 #8, 17(a, b, c, d)

8. $\{ (a, w), (w, a), (c, y), (y, c), (d, w), (w, d), (d, x), (x, d), (d, y), (y, d), (d, z), (z, d) \}$
17. a. $$
\begin{pmatrix}
1 & 1 & 1 & 1 \\
0 & 1 & 0 & 1 \\
0 & 0 & 1 & 0 \\
0 & 0 & 0 & 1
\end{pmatrix}
$$
b. $$
\begin{pmatrix}
0 & 0 & 0 & 0 \\
1 & 0 & 0 & 0 \\
1 & 1 & 0 & 0 \\
1 & 1 & 1 & 0
\end{pmatrix}
$$
c.$$
\begin{pmatrix}
3 & 2 & 1 & 0 \\
2 & 1 & 1 & 0 \\
1 & 1 & 0 & 0 \\
1 & 1 & 1 & 0
\end{pmatrix}
$$
d. $\{ (1,1),(1,2),(1,3),(2,1),(2,2),(2,3),(3,1),(3,2),(4,1),(4,2),(4,3) \}$
