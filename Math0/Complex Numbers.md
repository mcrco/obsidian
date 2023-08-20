# Question 1

Use the Euler equation to show

$$
\begin{gather}
\sin(\alpha+\beta) = \sin\alpha \cos\beta + \sin\beta \cos\alpha; \\
\cos(\alpha+\beta) = \cos\alpha \cos\beta -\sin\alpha \sin\beta
\end{gather}
$$

## Proof

Consider $e^{i(\alpha+\beta)}$. We can rewrite it as $e^{i\alpha} \cdot e^{i\beta}$. Expanding each factor, we get

$$
\begin{gather}
e^{i\alpha} = \cos\alpha + i\sin \alpha \\
e^{i\beta} = \cos\beta + i\sin\beta .
\end{gather}
$$

Now, multiplying the two factors,

$$
\begin{align}
e^{i\alpha} \cdot e^{i\beta} &= (\cos \alpha + i\sin \alpha)(\cos\beta + i\sin\beta) \\
&= \cos \alpha \cos\beta + i\sin\beta \cos\alpha + i\sin\alpha \cos\beta + i^{2}\sin \alpha \sin\beta \\
&= (\cos\alpha \cos\beta-\sin\alpha \sin\beta) + i(\sin\alpha \sin\beta+\sin\beta \sin\alpha)
\end{align}
$$

Since we know $e^{i(\alpha+\beta)}$ is also $\cos(\alpha+\beta) + i\sin(\alpha+\beta)$, we can equate

$$
\cos(\alpha+\beta) + i\sin(\alpha+\beta) = (\cos\alpha \cos\beta-\sin\alpha \sin\beta) + i(\sin\alpha \sin\beta+\sin\beta \sin\alpha).
$$

Equating the coefficients of the real and imaginary parts, we get

$$
\begin{gather}
\cos(\alpha+\beta) = \cos\alpha \cos\beta - \sin\alpha \sin\beta \\
\sin(\alpha+\beta) = \sin\alpha \sin\beta + \sin\beta \sin\alpha.
\end{gather}
$$

# Question 2

a. Show that $|z|=\text{Re}(z)$ iff $z$ is a non-negative real number.

## Proof

To prove that $|z|=\text{Re}(z)$ if and only if $z$ is a non-negative real number, we will prove the following 2 conditional statements:

1. If $z$ is a non-negative real number, then $|z|=\text{Re}(z)$ .
2. If $|z|=\text{Re}(z)$, $z$ is a non-negative real number. 

To prove the first statement, assume, $z$ is a non-negative real number. Thus $|z|=\sqrt{ z^{2}+0^{2} }=\sqrt{ z^{2} }$ since there is no complex part. $\sqrt{ z^{2} }$ is the absolute value of $z$, which is equal to $z$ when $z$ is non-negative. Because $z$ is the modulus and its own real part, if $z$ is non-negative real number, then $|z|=\text{Re}(z)$.

To prove the second statement, 

b.  