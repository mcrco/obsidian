- in relativistic physics, space and time are intertwined through [[Lorentz Transformation]]
- almost analogous to space and time being [[Finite Dimensional Vector Spaces#^c71fc8|bases]] for events
- different reference frame $\leftrightarrow$ rotation of $(x,y)$

![[Pasted image 20240118233313.png]]

$$
\begin{align}
x' &= (\cos\theta)x + (\sin\theta)x \\
y' &= -(\sin\theta)x + (\cos\theta)y
\end{align}
$$

- [[Lorentz Transformation]] is similar, almost like rotation of $xt$ frame

$$
\begin{align}
x' &= (\gamma)x - (\gamma V)t \\
t' &= -(\gamma V / c^{2}) + (\gamma)t
\end{align}
$$

- not perfect analogy tho, since
	- $\gamma,\gamma V,\gamma V / c$ can exceed unity (can't be sin/cos)
	- sign is different in $x'$ equation

# Minkowski Spacetime

- cannot separate space and time when discussing relativity
- need 4-dimensional **spacetime** to describe events
	- can't actually visualize 4 dimensions, but we can graph one or two dimensions of $x,y,z$ vs $ct$ (multiply time by speed of light so we can measure in meters)
	- called (1+dim) spacetime
- example graph of light ray in spacetime graph

![[Pasted image 20240123010433.png]]

- if we add another dimension $y$, we get a cone:

![[Pasted image 20240123010523.png]]

- this cone represents the absolute future and absolute past of observer at origin (events that affect observer must occur in this cone) since nothing travels faster than light
	- example: sun blew up 10 minutes ago in our frame of reference
	- sun is 8-light minutes away, so we can observe event
- events happening outside of cone cannot come into the cone and are called relative past and future
	- example: sun explodes 4 minutes ago in our reference frame at $t=0$
	- event doesn't reach us at $t=0$
	- thus it is in our relative past

![[Pasted image 20240123011418.png]]

- but at $t=4$ for us, it is in our absolute past

![[Pasted image 20240123011648.png]]

- light in (1+3) dimensional spacetime can be thought of as a sphere that expands and contracts as time evolves

# Intervals

## Comparison of 3D Space with 4D Spacetime

- in 3D space, displacement between $\mathbf{r}_{1}=(x_{1},y_{1},z_{1})$ and $\mathbf{r}_{2}=(x_{2},y_{2},z_{2})$ is $\mathbf{r}_{12}=(x_{1}-x_{2},y_{1}-y_{2},z_{1}-z_{1})$
- the distance $|\mathbf{r}_{12}|^{2}=(x_{2}-x_{1})^{2}+(y_{2}-y_{1})^{2}+(z_2-z_{1})^{2}>0$ if $\mathbf{r_{1}}, \mathbf{r_{2}}$ distinct
- also stays constant if we rotate coordinates/different reference frame
	- called an **invariant** under coordinate transformations
- in spacetime, $(x_{\mu})=(ct,x,y,z)$
	- $\mu=0,1,2,3$
	- $x_{\mu}$ changes when we change reference frames ([[Lorentz Transformation]])
- doesn't follow invariant square distance invariance of 3D vectors

$$
c^{2}t'^{2}+x'^{2}+y'^{2}+z'^{2}\neq c^{2}t^{2}+x^{2}+y^{2}+z^{2}
$$

- can prove by plugging in [[Lorentz Transformation]]
- however, using Lorentz,

$$
-c^{2}t'^{2}+x'^{2}+y'^{2}+z'^{2} = -c^{2}t^{2}+x^{2}+y^{2}+z^{2}
$$

- above equation implies spacetime is NOT Euclidean space
- intuition for equation: 
	- if light flashes at $(0,0,0,0)$ aka $x=0,y=0,z=0,t=0$
	- the light wave travels outwards in all directions $\implies$ sphere of radius $R=ct$, where $R^{2}=x^{2}+y^{2}+z^{2}$
	- thus,
	- $-c^{2}t^{2}+x^{2}+y^{2}+z^{2}=0$

## Spacetime Interval

- displacement in spacetime:

$$
(c\Delta t,\Delta x,\Delta y,\Delta z)
$$

- "Pythagorean Theorem" in spacetime:

$$
(\Delta s)^{2} \equiv -(c\Delta t)^{2} + (\Delta x)^{2} + (\Delta y)^{2} + (\Delta z)^{2}
$$

- $(\Delta s)^{2}$ is invariant
- can be negative, positive, zero
- $(\Delta s)^{2}>0$
	- **spacelike** since spatial separation dominates time separation
	- can always find frame of reference in which $\Delta t=0$ and events are simultaneous
	- can measure distance in this frame using distance alone (**proper length**)
	- $(\Delta s)^{2}=(\Delta l)^{2}=(\text{proper length})^{2}$
- $(\Delta s)^{2}<0$
	- **timelike**
	- can find frame in which $\Delta x=\Delta y=\Delta z=0 \implies$ events take place at same location
	- interval can be measured in time alone
	- $(\Delta s)^{2}\equiv -c^{2}(\Delta \tau)^{2})\equiv-c^{2}(\text{proper time})^{2}$
- $(\Delta s)^{2}=0$
	- **null**
	- corresponds to two events along some lightray, since the spatial separation is the same as the time separation times $c$