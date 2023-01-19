Solving for the electric field of a single particle is simple, but solving for the electric field with space is more challenging. To do this, we must enclose the space in a Gaussian shape and then use Gauss's Law:

$$
\phi_{E} = \oint \vec{E} d\vec{A} = \frac{Q_{enc}}{\epsilon_{0}}
$$

$\phi_{E}$ is the electric flux of the enclosed space across its surface, meaning Gauss's Law is a variation of a [[Parametric Surface and Surface Integral|Surface Integral]] or a [[Flux Integral]]. 

# Uniform Charge Density

## Electric Field Outside of Object

To demonstrate Gauss's Law in this situation, we take a cylinder with radius $R$, height $L$, and charge $Q$. 

$$
\begin{align}
\phi = \vec{E} d\vec{A} &= \frac{Q_{enc}}{\epsilon_{0}} \\
\implies \vec{E} \cdot 2\pi rL &= \frac{Q}{\epsilon_{0}} \\
\implies \vec{E} &= \frac{Q}{2\pi rL\epsilon_{0}}
\end{align}
$$

This holds true for both conductors and non-conductors.

## Electric Field Inside Object

### Conductors

Conductors have an internal electric field of 0.

### Non-Conductors

For this, we need the density of the charge, $\rho$. 

$$
\begin{align}
\vec{E} \cdot 2\pi rL &= \frac{Q_{enc}}{\epsilon_{0}} \\
\rho &= \frac{Q_{enc}}{V_{enc}} \\
&= \frac{Q}{\pi R^{2}L} \\
&= \frac{Q_{enc}}{\pi r^{2}L} \\
\implies Q_{enc} &= \frac{Qr^{2}}{R^{2}} \\
\implies \vec{E} &= \frac{Qr}{2\pi R^{2}L\epsilon_{0}}
\end{align}
$$

# Nonuniform Density

## 