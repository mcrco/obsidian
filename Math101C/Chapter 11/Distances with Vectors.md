# Point to Line

## Formula
$$
\frac{\vec{n}\cdot \vec{PQ}}{\lvert \lvert \vec{n} \rvert \rvert }
$$

## Derivation

Given a line $L$ in the form $ax + by + c = 0$ and a point $P$, the distance between the point and the line is just the component of the vector $\vec{PQ}$, where $Q$ is an arbitrary point on the line, and $\vec{n}$, the normal vecvtor of $L$.

$$
\begin{align}
\vec{n} &= <a, b> \\
D &= comp_{\vec{n}}\vec{PQ} \\
&= \frac{\vec{n}\cdot \vec{PQ}}{\lvert \lvert \vec{n} \rvert \rvert } \\
\end{align}
$$

# Point to Vector

## Formula
$$
\frac{\lvert \lvert \vec{PQ}\times \vec{v} \rvert \rvert }{\lvert \lvert \vec{v} \rvert \rvert }
$$

## Derivation

Given a line as a parametric function that we can write as a vector and a point, we can find the distance between the point and the line as the magnitude of the vector connecting the point to any point on the line multiplied by the sine of the angle it forms with the line's parallel vector.

Let $P$ be a point, let $\vec{v}$ be the line's vector, and let $Q$ be a point on the line.

$$
\begin{align}
D &= \lvert \lvert \vec{PQ} \rvert \rvert \sin \theta \\
&= \lvert \lvert \vec{PQ} \rvert \rvert \frac{\lvert \lvert \vec{PQ}\times \vec{v} \rvert \rvert }{\lvert \lvert \vec{PQ} \rvert \rvert \lvert \lvert \vec{v} \rvert \rvert } \\
&= \frac{\lvert \lvert \vec{PQ}\times \vec{v} \rvert \rvert }{\lvert \lvert \vec{v} \rvert \rvert }
\end{align}
$$

# Point to Plane

## Formula

$$

$$

We can use the same approach as [[#Point to Line]]. 


# Plane to Plane