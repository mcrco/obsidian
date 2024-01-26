- a vector space over a [[Fields|field]] $F$ is a [[Sets|set]] of of vectors where
	- addition is [[Vectors#^cbddf2]] 
	- multiplication is [[Vectors#^85a8b3]] 
- and satisfies the below axioms

# Addition

> [!axiom] Commutativity
> %% label: commutativity %%
> $\vec{u}+\vec{v}=\vec{v}+\vec{u}$.

> [!axiom] Associativty
> %% label: associativty %%
> $(\vec{u}+\vec{v})+\vec{w}=\vec{u}+(\vec{v}+\vec{w})$.

> [!axiom] Zero Vector
> %% label: zero-vector %%
> Exists a vector $\vec{0}$ s.t. $\vec{v}+\vec{0}=\vec{v}$.

> [!axiom] Additive Inverse
> %% label: additive-inverse %%
> $\forall \, \vec{v} \in V$, $\exists \, \vec{w}$ s.t. $\vec{v}+\vec{w}=\vec{0}$. $\vec{w}=-\vec{v}$.

^7661b4

## Multiplication

> [!axiom] Multiplicative Identity
> %% label: multiplicative-identity %%
> $\exists \, 1 \in V$ s.t. $1\vec{u} = \vec{u}$.

> [!axiom] Multiplicative Associativity
> %% label: multiplicative-associativity %%
> For scalars $c,d$, $c(d\vec{u}) = (cd)\vec{u}$.

# Distribution

- connects addition and multiplication

> [!axiom] First Distribution
> %% label: first-distribution %%
> $c(\vec{u} + \vec{v}) = c\vec{u} + c\vec{v}$.

> [!axiom] Second Distribution
> %% label: second-distribution %%
> $(c + d)\vec{u} = c\vec{u} + d\vec{u}$.

# Examples

- vector spaces over $\mathbb{R}$
	- $V=\mathbb{R}^{2}$
	- $V=\{ f:\mathbb{R}\to\mathbb{R} \}$
	- $V=\{ \text{continuous }f:\mathbb{R}\to\mathbb{R} \}$
	- $V=\{ p(x)=a_{0}+a_{1}x+\dots+a_{n}x^{n} \}$ where $a_{0},\dots a_{n}\in\mathbb{R}$
	- For field $K$, $K^{n}=\{ (a_{1},a_{2}, \dots, a_{n}) \} | a_{i} \in K$
		- $K-$vector space

# Subspace

> [!definition] Vector Subspace
> %% label: vector-subspace %%
> If $V$ is a $K-$vector subspace then a subspace of $V$ is a subset $W \subset V$ s.t. $W$ is also a $K-$vector space using the same operations.

> [!definition] Closure under Operation
> %% label: closure-under-operation %%
> A subset $S \subset V$ is closed under $\star$ if given $\vec{s}_{1}, \vec{s}_{2} \in S$ then $\vec{s}_{1}\star\vec{s_{2}}\in S$.

- vector spaces are also closed under addition and scalar multiplication, but didn't have to define since [[Vectors#^cbddf2|addition]] and [[Vectors#^85a8b3|multiplication]] are [[Vectors#^aed3cb|binary operations]] and closing by default
- notice that

> [!proposition]
> Nonempty $W \subset V$ is subspace $\iff$ $W$ is closed under addition and scalar multiplication

## Axioms

> [!axiom]
> $\vec{0} \in W$ always.

`\begin{proof}`For any $\vec{w} \in W$, $0 \cdot \vec{w}=\vec{0} \implies \vec{w} \in W$.`\end{proof}`

> [!axiom]
> [[#^7661b4|Additive Inverse]] $\in W$ always
> 

`\begin{proof}`For any $\vec{w} \in W$, $-1 \cdot \vec{w} = -\vec{w}$. `\end{proof}`

## Subspaces of $\mathbb{R}^{2}$

- if $W$ is subspace, then
- $\vec{w} \in W \neq \vec{0} \implies \lambda \vec{w} \in W$ for $\lambda \in \mathbb{R}$
- $L=\{ \lambda \cdot \vec{w} \mid \lambda \in \mathbb{R} \}$ is subspace (check for closure)
	- $L$ is actually just a line through $\vec{0}$ if visualized on plane

> [!claim]
> If $W \subset V$ is a subspace, it's either $\vec{0}, \mathbb{R}^{2}$, or line through $\vec{0}$.

`\begin{proof}`Given $W$, assume it's not $\{ \vec{0} \}$
`\end{proof}`

> [!claim]
> Given any $\vec{u} \in \mathbb{R}^{2}$, can write $\vec{u}=\lambda \vec{w} + \mu \vec{v}$ for unique $\lambda,\mu$

