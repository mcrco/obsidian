# p. 335, #14, 15, 20, 26

14. $A_{0} = 3000$
15. $A_{1} = 3360, A_{2} = 3736.2, A_{3} = 4214.78$
20. We use induction. The base case is that $S_{1} = f_{3} = 2$, which is true since there are only 2 one bit strings. Our inductive step is that for every case after $n=1$, the number of valid strings is just the sum of the number of valid strings with 1 less bit and the number of vlaid strings with 2 less bits. We can use casework to prove this. If we want a valid string of length $n$ to end in a 1, we can just take any valid string of length $n-1$ and add a 1 to the end. If we want a valid of string of length $n$ to end in a 0, we can just take any valid string of length $n-2$ and add 10 to the end of it to ensure there are no consecutive 0s. 
26. We can plug in values to show the base case works for $C_{0}, C_{1}, C_{2}$. For our induction, we can use the formula for $C_{n+1}$ and derive the recursion:
$$
\begin{align}
C_{n} &= \frac{1}{n+1} {2n \choose n}  \\
C_{n+1} &= \frac{1}{n+2} {2(n+1) \choose n+1}  \\
(n+2) C_{n+1} &= \frac{(2n+2)!}{(n+1)!(n+1)!} \\
&= \frac{(2n+2)(2n+1)(2n)!}{(n+1)^{2}(n!)^{2}} \\
&= \frac{(2n+2)(2n+1)}{(n+1)^{2}}{2n \choose n}  \\
&= (4n+2){2n \choose n} 
\end{align}
$$

# p. 347, 1-10, 15, 17, 36, 37, Choose one of 41-43

1. order of 1
2. non constant coefficients
3. non constant coefficients
4. order of 1
5. non constant coeff
6. order of 3
7. non constant coeff
8. order of 2
9. order of 2
10. order of 3
15. $$
\begin{align}
a_{n} &= r^{n} \\
r^{n} &= 6r^{n-1} - 8r^{n-2} \\
r &= 2, 4 \\
a_{n} &= b 2^{n} + c 4^{n} \\
\end{align}
$$
Plugging in given conditions, we get

$$
\begin{align}
1 &= b + c \\
0 &= 2b + 4c \\
c &= -1 \\
b &= 2 \\
a_{n} &= 2\cdot 2^{n} -4^{n}
\end{align}
$$

17. $$
\begin{align}
r &= 2, 5 \\
a_{n} &= b 2^{n} + c 5^{n} \\
5 &= b + c \\
16 &= 2b + 5c \\
c &= 2 \\
b &= 3 \\
a_{n} &= 3\cdot 2^{n} + 2 \cdot 5^{n}
\end{align}
$$

36. $$
\begin{align}
r &= 2, -1 \\
1 &= b + c \\
1 &= 2b - c \\
b &= \frac{2}{3} \\
c &= \frac{1}{3} \\
b_{n} &= \frac{2}{3} \cdot 2^{n} + \frac{1}{3}\cdot(-1)^{n} \\
a_{n} &= (\frac{2}{3} \cdot 2^{n} + \frac{1}{3}\cdot(-1)^{n})^{2}
\end{align}
$$

37. $$
\begin{align}
b_{n} &= \frac{1}{2}b_{n-2} - \frac{1}{2}b_{n-1} \\
r &= -1, \frac{1}{2} \\
b_{n} &= c(-1)^{n} + d\left( \frac{1}{2} \right)^{n} \\
\log 8 &= c + d \\
- \log 2\sqrt{ 2 } &= -c + \frac{1}{2}d \\
d &= \frac{2}{3}\log 2\sqrt{ 2 } \\
c &= \frac{4}{3}\log 2\sqrt{ 2 } \\
b_{n} &= \frac{4}{3} \log 2\sqrt{ 2 }(-1)^{n} + \frac{2}{3} \log 2\sqrt{ 2 }\left( \frac{1}{2} \right)^{n} \\
a_{n} &= \frac{4}{3}(-1)^{n} + \frac{2}{3}\left( \frac{1}{2} \right)^{n}
\end{align}
$$
# Proof

Show that $C_{n} > 2n, n\geq 1$

$$
\begin{align}
C_{n} &= \frac{1}{n+1}{2n \choose n}  \\
&= \frac{1}{n+1}\cdot\frac{2n\cdot(2n-1)\cdot(2n-2)\dots}{n(n-1)(n-2)\dots} \\
&= \frac{1}{n+1}\cdot \frac{2n}{n} \cdot \frac{2n-1}{n-1} \cdot \frac{2n-2}{n-2} \dots
\end{align}
$$

Since every term to the right of $\frac{1}{n+1}$ in the expression for $C_{n}$ is greater than 2, we know

$$
C_{n} > \frac{1}{n+1} 2^{n}
$$

We use induction to prove the term on the right is greater than 2. Our base case is

$$
C_{1} = \frac{1}{1+1}2^{1} = 1
$$

Nevermind it's not true, I just plugged in values for $C_{1}$. But I'm not gonna erase all the beautiful LaTex I just wrote.