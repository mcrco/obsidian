# Energy and Inertia

- after special relativity, Einstein proposed that inertia of object depended on energy
	- inertia: reluctance of object to change state of motion
- deduced $E=mc^{2}$
- how?

## Thought Experiment

- imagine massless cardboard tube of length $L$ with metal caps on each end of mass $m$

![[Pasted image 20240125142435.png]]

- now, imagine light is emitted from left cap towards right cap
- light beam has small energy $\Delta E$ and small momentum $\Delta p=\Delta E / c$
- thus, to conserve momentum, tube has to shift to the left until light is reabsorbed by right cap

![[Pasted image 20240125143013.png]]

- solving for the velocity of the tube (non-relativistic btw since it is very small)

$$
\Delta v_{\text{tube}} = \frac{\Delta p}{2m} = \frac{\Delta E}{2mc}
$$

- solving for shift in position,

$$
\Delta x = \Delta v_{\text{tube}}t = \frac{\Delta E}{2mc} \frac{L}{c} = \frac{\Delta EL}{2mc^{2}}
$$

- remember that light has no mass
- that means the tube changed center of mass... without an external force?!?!?!??!
- doesn't make sense, so now suppose light **does** have mass $\Delta m$, and that the left cap loses $\Delta m$ and the right cap gains $\Delta m$
- to keep center of mass the same, the mass times distance from COM on each end should equate:

$$
(m-\Delta m)(L/ 2 + \Delta x) = (m+\Delta m)(L/2 - \Delta x) 
$$

- above reduces to

$$
2m\Delta x = \Delta mL 
$$

- plugging in $\Delta x$ and solving for $\Delta m$,

$$
\Delta m =\frac{\Delta E}{c^{2}}
$$

- or, as the famous equation goes

$$
\Delta E=\Delta mc^{2}
$$

# Energy Momentum Four Vector

## Energy to Collisions

- to fully understand $E=mc^{2}$, think back to collisions
- remember the formula for [[Momentum in Relativistic Physics#Momentum in 4D Spacetime|relativistic momentum]]

$$
(p_{\mu}) = (\gamma mc, \mathbf{p})
$$

- and our [[Momentum in Relativistic Physics#Summary|question about the zeroth component]]: what is first term $p_{0}$?
- collisions can either be elastic or inelastic (energy is conserved or not conserved)
	- $\implies$ if collision is elastic in one frame and energy is conserved, it must be conserved in all frames
- thus, maybe $p_{0}$ is energy???
	- "but $p_{0}=\gamma mc$ isn't in energy units!"
	- we can simply multiply $p_{0}$ by $c$ to get $E=p_{0}c=\gamma mc^{2}$
		- seems familiar to $E=mc^{2}$

## Validating

- suppose particle is at rest
	- $v=0 \implies \gamma=1$

$$
E_{0}=mc^{2}
$$

- exact same formula as thought experiment
- if particle is moving, energy increases
	- makes sense cuz kinetic energy increases with velocity in classical mechanics
- kinetic energy redefined as 

$$
KE=E-E_{0}=\gamma mc^{2}-mc^{2}=mc^{2}(\gamma-1) = mc^{2}\left( \frac{1}{\sqrt{ 1-v^{2}/c^{2} }} -1\right)
$$

- if particle has small velocity $v / c \ll 1$, we can use binomial expansion

$$
(1+x)^{n}=1 + nx + {n \choose 2} x^{2} + {n \choose 3} x^{3} + \dots
$$

- and use the fact that it converges fast if $|x| = v^{2} / c^{2} \ll 1$ to approximate

$$
(1-v^{2} / c^{2})^{-1 / 2} = 1+ \frac{1}{2} \frac{v^{2}}{c^{2}} + \dots
$$

- thus,

$$
\begin{align}
KE&=mc^{2}\left( \frac{1}{\sqrt{ 1-v^{2} / c^{2} }}-1 \right) = mc^{2}\left( 1+ \frac{1}{2} \frac{v^{2}}{c^{2}} + \dots - 1 \right) \\
&= \frac{1}{2}mv^{2} + \dots
\end{align}
$$

 - biggest term is non-relativistic KE (notice if we approximate $v / c \ll 1$, it's equal)

$$
E = \gamma mc^{2} = \frac{mc^{2}}{\sqrt{ 1-v^{2} / c^{2} }}
$$

-  reduces to classical KE if $v / c \ll 1$
- when checking if transformation under [[Lorentz Transformation]] is consistent, experiments prove it is
- plugging into Lorentz invariant,

$$
-p_{0}^{2} + p_{x}^{2} + p_{y}^{2} + p_{z}^{2} = -(E / c)^{2} + p_{x}^{2} + p_{y}^{2} + p_{z}^{2}
$$

- then, solving for $E$,

$$
\begin{align}
-(E / c)^{2} + p_{x}^{2} + p_{y}^{2} + p_{z}^{2} &= -\gamma^{2}m^{2}c^{2}+\gamma^{2}m^{2}v^{2} \\
&= -\gamma^{2}m^{2}c^{2}(1-v^{2} / c^{2}) \\
&= -m^{2}c^{2}
\end{align}
$$

- thus,

$$
E^{2} = p^{2}c^{2} + m^{2}c^{4}
$$

# Decay of Particle Example

- suppose particle of mass $M$ breaks up into 2 identical pieces of mass $m$
	- actual nature example: $K^{0} \to \pi^{0} + \pi^{0}$

![[Pasted image 20240126001000.png]]

- momentum is conserved, so pieces move at opposite velocity $v$ (as shown above)
- energy is conserved
	- $E_{i} = Mc^{2}$
	- $E_{f}=2mc^{2} / \sqrt{ 1-v^{2} / c^{2} }$

$$
M = \frac{2m}{\sqrt{ 1-v^{2}/c^{2} }}
$$

- mass isn't conserved since $M > 2m$
- $\therefore$ mass must've converted to energy

> [!remark]
> Two classical laws of conservation (mass and energy) have now been merged into one relativistic law of conservation of energy (mass energy and kinetic energy).

- solving for speed of particles, we get

$$
\frac{v}{c} = \sqrt{ 1-\frac{4m^{2}}{M^{2}} }
$$

- it will be more convenient to $v / c$ for $K^{0}\to \pi^{0}+\pi^{0}$ if we first define

# Energy Units

- atomic, nuclear, particle physics uses **electron volt** (eV)
- one eV is energy gained by electron in electric field with potential difference of 1 volt

$$
1\text{ eV} = 1.60 \times 10^{-19} \text{ J}
$$

