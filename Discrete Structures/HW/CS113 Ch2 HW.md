# p70 7, 13, 16, 19, 23, 31, 45

7. **Claim**: If $m$ and $n$ are even, $m + n$ is even
**Proof**:
Let $m = 2a$ and $n = 2b$ by the definition of an even number.
Then
$$
\begin{align}
m + n &= 2a + 2b \\
&= 2(a + b)
\end{align}
$$
The above shows that $m + n$ must be even since $2(a + b)$ is an even number by definition.

13. Claim: For all rational number $x$ and $y$, $x + y$ is rational.
Let $x = \frac{a}{b}, y = \frac{c}{d}$, where $a, b, c, d$ are all integers.

$$
x + y = \frac{ad + bc}{bd} 
$$

Since we know that the sum and products of integers are also integers, we get that $\frac{ad + bc}{bd}$ must be rational as well since it has an integer numerator and denominator.

16.  Claim: The product of two integers, one of the form $3k_{1} + 1$ and the other of the form $3k_{2} + 2$, where $k_{1}$ and $k_{2}$ are integers, is of the form $3k_{3} + 2$ for some integer $k_{3}$ .

$$
\begin{align}
(3k_{1} + 1)(3k_{2} + 2) &= 9k_{1}k_{2} + 3k_{1} + 3k_{2} + 2 \\
&= 3(3k_{1}k_{2} + k_{1} + k_{2}) + 2
\end{align}
$$

Letting $k_{3} = 3k_{1}k_{2} + k_{1} + k_{2}$, we prove the claim to be true.

19. Setting the 3 theorems to T1, T2, and T3, respectively, we get that they are used in the proof in the order T1, T2, T3.

23. $\{ n|n\in\mathbb{Z}^{+}, n > 5 \}$

31. 5

45. Both 1 and 2 fit into the condition equation of $B$, so $A$ must be a subset of $B$. 

# p81 12, 35, 47

12. We just have to find one example of $x^{y}$ being rational. Casework. $a^{b}$ is rational because $2^{\sqrt{ 2 }^{\sqrt{ 2 }}} = \sqrt{ 2 }^{2} = 2$, which is rational.

35. Claim: The product of two consecutive numbers is even.
Let the 2 numbers be $n$ and $n + 1$. 
Case 1: $n$ is even

$$
\begin{align}
n &= 2p \\
n(n + 1) &= 2p(2p + 1) \\
&= 2(2p^{2} + p)
\end{align}
$$

This must be even by the definition of an even number

Case 2: $n$ is odd

$$
\begin{align}
n &= 2p + 1 \\
n(n + 1) &= (2p + 1)(2p + 2) \\
&= 2(2p + 1)(p + 1)
\end{align}
$$

This must also be even by definition.

47. Claim: $n$ is odd iff $n + 2$ is odd.
Part 1: $n+2$ is odd => $n$ is odd

$$
\begin{align}
n + 2 &= 2p + 1 \\
n &= 2p - 1 \\
&= 2(p - 1) + 1
\end{align}
$$

$n$ is odd by definition is $n + 2$ is odd.
Part 2: $n$ is even => $n + 2$ is even

$$
\begin{align}
n &= 2p \\
n + 2 &= 2p + 2 \\
&= 2(p + 1)
\end{align}
$$

$n + 2$ is even by definition, meaning that $n$ must also be odd if $n + 2$ is odd.

# p96 2, 3, 4, 16, 22

2. $1 \cdot 2 + 2 \cdot 3 \dots + n(n + 1) = \frac{n(n + 1)(n + 2)}{3}$

Base Case: 

$$
\begin{align}
S(1): 1 \cdot (1 + 1) &= \frac{1(1 + 1)(1 + 2)}{3} \\
2 &= 2
\end{align}
$$

Induction:

$$
\begin{align}
S(n) + (n + 1)(n + 2) &= \frac{n(n + 1)(n + 2)}{3} + (n + 1)(n + 2) \\
&= \frac{(n + 1)(n + 2)(n + 3)}{3} \\
&= S(n + 1)
\end{align}
$$

3. $1(1!) + 2(2!) + \dots + n(n!) = (n + 1)! - 1$

Base Case:

$$
\begin{align}
S(1): 1(1!) &= (1 + 1)! - 1 \\
1 &= 1
\end{align}
$$

Induction: 

$$
\begin{align}
S(n) + (n + 1)(n + 1)! &= (n + 1)! - 1 + (n + 1)(n + 1)! \\
&= (n + 2)(n + 1)! - 1\\
&= (n + 2)! - 1 \\
&= S(n + !)
\end{align}
$$

4. $1^{2} + 2^{2} \dots + n^{2} = \frac{n(n + 1)(2n + 1)}{6}$

Base Case:

$$
\begin{align}
S(1): 1^{2} &= \frac{1(1 + 1)(2n + 1)}{6} \\
1 &= 1
\end{align}
$$

Induction:

$$
\begin{align}
S(n) + (n + 1)^{2} &= \frac{n(n + 1)(2n + 1)}{6} + (n + 1)^{2} \\
&= \frac{(n + 1)(6(n + 1) + n(2n + 1))}{6} \\
&= \frac{(n + 1)(n + 2)(2n + 3)}{6} \\
&= S(n + 1)
\end{align}
$$

16. $2^{n} \geq n^{2}$, $n = 4, 5, \dots$

Base Case:

$$
\begin{align}
S(3): 2^{4} &\geq 4^{2} \\
16 &\geq 16
\end{align}
$$

Induction:

$$
\begin{align}
2^{n + 1} &\geq (n + 1)^{2} \\
2 \cdot 2^{n} &\geq n^{2} + 2n + 1 \\
2^{n} + 2^{n} &\geq n^{2} + 2n + 1
\end{align}
$$

Since we assume that $2^{n} \geq n^{2}$ from the base case and $2^{n} \geq 2n + 1$  from the given conditions, the inductive step is true.

22. $7^{n} - 1 = 6k, n \geq 1$

Base:

$$
\begin{align}
S(1): 7^{1} - 1 &= 6k \\
6 &= 6(1)
\end{align}
$$

Induction:

$$
\begin{align}
S(n + 1) &= 7^{n + 1} - 1 \\
&= 7 \cdot 7^{n} - 1 \\
&= 7 \cdot (6k + 1) - 1 \\
&= 42k + 7 - 1 \\
&= 6(7k + 1)
\end{align}
$$

$S(n + 1)$ must be divisible by 6.