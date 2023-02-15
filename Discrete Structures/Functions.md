- definition: one-way correspondence between two sets
- examples
	- mod function
		- $k\mod m: k \in \mathbb{R} \to \{ n| n \in Z, 0 \leq n < m \}$
	- hash function
		- uses mod function
	- LCG

# Types of Functions

## Injective

- also called 1-1
- 1 output for very input

### Demonstration

$f(x)=2x+3$ is injective.

Proof by contradition:

$$
\begin{align}
f(a) &= f(b)\\
2a + 3 &= 2b + 3 \\
\implies a &= b
\end{align}
$$

Clearly there is only one x per y.

## Surjective

- also called onto
- at least one 1 input for every output

### Demonstration

$f(x)=x^{2}$ is surjective but not injective for $D: \{ x|x\in\mathbb{R} \}$, $R:\{ y|y\in\mathbb{R} \}$

