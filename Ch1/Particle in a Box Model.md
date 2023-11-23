Simple but important model that develops physical understanding of chemical applications of quantum mechanics.

# One-Dimensional Boxes

- simplest model problem for which [[Quantum Mechanics#Schrodinger's Equation]] can be solved
- particle confined by potential energy barriers with infinite potential energy
	- particle only exists in certain region of box
	- one dimension $\implies$ bead slides along wire between barriers at ends of wires
 
![[Pasted image 20231122214950.png]]

- potential energy inside box is $V(x)=0$, thus
- total energy must be $E = T+V > 0$ inside box
- we can use these constraints to solve for all possible energy levels $E$

Since it's impossible to find particle outside of box, 

$$
P(x) = \psi^{2}(x) = 0 \implies \psi(x) = 0.
$$

Inside the box, $V=0$, so Schrodinger's equation becomes

$$
-\frac{h^{2}}{8\pi^{2}m} \frac{d^{2}\psi(x)}{dx^{2}} = E\psi(x).
$$

The LHS is usually simplified with the Hamiltonian operator $\hat{H}$, which gives us the classic

$$
\hat{H}\psi = E\psi.
$$

Back to the previous equation: we can simplify it to become

$$
\frac{d^{2}\psi(x)}{dx^{2}} = -\frac{8\pi^{2}mE}{h^{2}}\psi(x).
$$

Since this is a [[Differential Equation]], we know that sine and cosine are solutions for $\psi$.


