# Comparison to Classical Momentum

- say classical momentum is $\mathbf{p} = m\mathbf{v}$ for frame $S$
- when changing frame to $S'$ moving at velocity $\mathbf{V}$, we apply Galilean velocity transform to get $\mathbf{p}'=m\mathbf{v}'=m(\mathbf{v}-\mathbf{V})$
- thus, if momentum is conserved in $S$ for group of particles, it is conserved in $S'$ since the factor of $\mathbf{V}$ is added everywhere
- however, in relativity, we [[Lorentz Transformation#Velocity Transformation|transform velocity between frames]]

$$
v_{x} = \frac{v_{x}'+V}{1+v_{x}'V / c^{2}}
$$

- thus, collision in frame $S$ can have

$$
m_{a}v_{ai} + m_{b}v_{bi} = m_{a}v_{af} + m_{b}v_{b f}
$$

- but same collision in frame $S'$ with transformed velocities, each velocity scales differently according to factor in denominator of transform

$$
m_{a}v_{ai}' + m_{b}v_{bi}' \neq m_{a}v_{af}' + m_{b}v_{b f}'
$$
# Momentum in 4D [[Spacetime]]

- we need to find a 4-vector with invariance like $\Delta s^{2}$ like in [[Spacetime#Spacetime Interval|spacetime intervals]]
- classical momentum is 

$$
\mathbf{p}=m \frac{d}{dt} (x,y,z) = \left( m \frac{dx}{dt}, m \frac{dy}{dt}, m \frac{dz}{dt} \right)
$$

- similarly, four-vector momentum is

$$
{p}_{\mu} = m \frac{d}{d\tau} (ct, x, y, z) = \left( mc \frac{dt}{d\tau}, m \frac{dx}{d\tau}, m \frac{dy}{d\tau} m \frac{dz}{d\tau} \right)
$$

- plugging in the formula for [[Intro to Special Relativity#Time Dilation|time dilation]], $\Delta \tau = \Delta t\sqrt{ 1-v^{2} / c^{2} }$, we get 

$$
\lim_{ \tau \to 0 } \frac{\Delta t}{\Delta \tau}= \frac{dt}{d\tau}= \frac{1}{\sqrt{ 1-  v^{2} / c^{2} }}
$$

- using chain rule on velocity, we get

$$
\frac{dx}{d\tau} = \frac{dt}{d\tau} \frac{dx}{dt} = \frac{1}{\sqrt{ 1 - v^{2}/ c^{2} }} v_{x}
$$

- using $\mathbf{v}=(\frac{dx}{dt}, \frac{dy}{dt}, \frac{dz}{dt})$,

$$
(p_{\mu}) = \left( \frac{mc}{\sqrt{ 1-v^{2} / c^{2} }}, \frac{m\mathbf{v}}{\sqrt{  1 - v^{2} / c^{2} }} \right)
$$

- let $\gamma_{L} = \frac{1}{\sqrt{ 1-  v^{2} / c^{2} }}$
	- Lorentz factor
	- different from $\gamma$ in [[Lorentz Transformation]] since here $v$ is speed of particle, not frame
- then,

$$
\mathbf{p} = \gamma m\mathbf{v}
$$

- above is universal expression for momentum of any particle
	- reduces to classical expression $\mathbf{p}=m\mathbf{v}$ when $v\ll c$
- we can validate that above expression stays constant in any inertial frame by first assuming

	$$
(P_{\mu})_{\text{initial}} = (P_{\mu})_{\text{final}}
$$

- then applying [[Lorentz Transformation]] with a frame moving at velocity $V$ in the $x$ direction to every component of four-momentum

$$
\begin{align}
P_{0}' &= \gamma_{L}(P_{0}-VP_{x} / c) \\
P_{x}' &= \gamma(P_{x} - VP_{0} / c) \\
P_{y}' &= P_{y} \\
P_{z}' &= P_{z}
\end{align}
$$

- thus, if $(P_{\mu})_{\text{initial}}=(P_{\mu})_{\text{final}}$, we can substitute the values into $(P_{\mu})'$ to get that 

$$
(P_{\mu})_{\text{initial}}' = (P_{\mu})_{\text{final}}'
$$

## Summary

- four-momentum $(p_{\mu})$ has passed 2 important tests:

1. spatial components of $p_{\mu}$ reduce to classical $p$ for small velocities
2. total momentum of system is conserved in all inertial frames if it is conserved in one initial frame

- however, still need to figure out if

1. momentum is conserved in collisions of relativistic particles
2. what is meaning of time component
3. what is the meaning of invariant quantity