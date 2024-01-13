To transform [[Intro to Special Relativity#Implications]] between reference frames, we use the Lorentz Transformation.

# The Transformation

## Galilean Form

$$
\begin{align}
x' &= x - vt \\
t' &= t \\
\end{align}
$$

## Lorentz

$$
\begin{cases}
x' = \gamma(x-vt) \\
t' = \gamma\left( t-\frac{vx}{c^{2}} \right)
\end{cases} \to \begin{cases}
x' = \gamma(x-\beta c t) \\
ct' = \gamma\left( ct-\beta x \right)
\end{cases}
$$

- $\frac{1}{\gamma^{2}}+\beta^{2}=1$ by definition in [[Intro to Special Relativity#Significance]]

Notice this is just a [[Linear Transformations|linear transformation]]:

$$
\begin{pmatrix}
x' \\
ct'
\end{pmatrix}
= \begin{pmatrix}
\gamma  & - \beta\gamma \\
-\beta\gamma & \gamma
\end{pmatrix}\begin{pmatrix}
x \\
ct
\end{pmatrix}
.$$


# Time Dilation

- observe a person moving at $v=\beta c$ for a time $t$ 
- applying the transformation to get their time:

$$
\begin{align}
ct'&=\gamma ct-\beta\gamma x \\
&= \gamma ct-\beta\gamma(\beta ct) \\
&= \gamma(1-\beta^{2})ct \\
\implies t' &= \frac{t}{\gamma}.
\end{align}
$$

# Velocity Transformation

- now observe the same person, but we move at velocity $u$
- transform/boost velocity:

$$
\begin{align}
u_{x}'&=\frac{dx'}{dt'} \\
&=\frac{dx'}{dt}\left( \frac{dt}{dt'} \right)  \\
&= \frac{dx' / dt}{dt' / dt}  \\
&= \frac{\gamma(u-\beta c)}{\gamma\left( 1-\frac{\beta u}{c} \right)} \\
&= \frac{u-v}{1-\frac{vu}{c^{2}}}
\end{align}
$$

- in two dimensions $x,y$
	- person still only moves in $x$

$$
\begin{align}
u_{x}'&= \frac{u_{x}-v}{1-\frac{vu_{x}}{c^{2}}} \\
u_{y}'&= \frac{uy}{\gamma\left( 1-\frac{\beta u_{x}}{c} \right)}
\end{align}
$$

- now imagine two spaceships moving towards each other at $0.99c$ and $-0.99c$
- velocity greater than $c$?!
- no lol
- if we (static observer of event) boost to $0.99c$
	- $v=0.99c$
	- $u=-0.99c$

$$
\begin{align}
u' &= \frac{-0.99c - 0.99c}{1-\frac{(0.99)(-0.99)c^{2}}{c^{2}}} \\
&= -\frac{1.98c}{1.9801} \\
&= -0.99995c
\end{align}
$$

# Intervals

- $(ct,x,y,z)$: location in spacetime (event)

$$
\Delta s^{2}=-(c\Delta t)^{2}+(\Delta x)^{2}+(\Delta y)^{2}+(\Delta z)^{2}
$$

- if only $x$, can visualize events $A,B,C,D,E$ as

![[Pasted image 20240111115723.png]]

- $C-D$: $\Delta s^{2}=0 \implies$ null
- $A-B$: $\Delta s^{2}>0 \implies$ time-like
- $C-D$: $\Delta s^{2}<0 \implies$ space-like