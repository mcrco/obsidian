- a vector space over a [[Fields|field]] $F$ is a set of of vectors where
	- addition is [[Vectors#^cbddf2]] 
	- multiplication is [[Vectors#^85a8b3]] 
- and satisfies the below axioms

# Addition

> [!math|{"type":"axiom","number":"auto","setAsNoteMathLink":false,"title":"Commutativity","label":"commutativity","_index":0}] Axiom 1 (Commutativity).
> $\vec{u}+\vec{v}=\vec{v}+\vec{u}$.

> [!math|{"type":"axiom","number":"auto","setAsNoteMathLink":false,"title":"Associativty","label":"associativty","_index":1}] Axiom 2 (Associativty).
> $(\vec{u}+\vec{v})+\vec{w}=\vec{u}+(\vec{v}+\vec{w})$.

> [!math|{"type":"axiom","number":"auto","setAsNoteMathLink":false,"title":"Zero Vector","label":"zero-vector","_index":2}] Axiom 3 (Zero Vector).
> Exists a vector $\vec{0}$ s.t. $\vec{v}+\vec{0}=\vec{v}$.

> [!math|{"type":"axiom","number":"auto","setAsNoteMathLink":false,"title":"Additive Inverse","label":"additive-inverse","_index":3}] Axiom 4 (Additive Inverse).
> $\forall \, \vec{v} \in V$, $\exists \, \vec{w}$ s.t. $\vec{v}+\vec{w}=\vec{0}$. $\vec{w}=-\vec{v}$.

## Multiplication

> [!math|{"type":"axiom","number":"auto","setAsNoteMathLink":false,"title":"Multiplicative Identity","label":"multiplicative-identity","_index":4}] Axiom 5 (Multiplicative Identity).
> $\exists \, 1 \in V$ s.t. $1\vec{u} = \vec{u}$.

> [!math|{"type":"axiom","number":"auto","setAsNoteMathLink":false,"title":"Multiplicative Associativity","label":"multiplicative-associativity","_index":5}] Axiom 6 (Multiplicative Associativity).
> For scalars $c,d$, $c(d\vec{u}) = (cd)\vec{u}$.

# Distribution

- connects addition and multiplication

> [!math|{"type":"axiom","number":"auto","setAsNoteMathLink":false,"title":"First Distribution","label":"first-distribution","_index":6}] Axiom 7 (First Distribution).
> $c(\vec{u} + \vec{v}) = c\vec{u} + c\vec{v}$.

> [!math|{"type":"axiom","number":"auto","setAsNoteMathLink":false,"title":"Second Distribution","label":"second-distribution","_index":7}] Axiom 8 (Second Distribution).
> $(c + d)\vec{u} = c\vec{u} + d\vec{u}$.

# Examples

- vector spaces over $\mathbb{R}$
	- $V=\mathbb{R}^{2}$
	- $V=\{ f:\mathbb{R}\to\mathbb{R} \}$
	- $V=\{ \text{continuous }f:\mathbb{R}\to\mathbb{R} \}$
	- $V=\{ p(x)=a_{0}+a_{1}x+\dots+a_{n}x^{n} \}$ where $a_{0},\dots a_{n}\in\mathbb{R}$

# Subspace

- subset of vector space that is also a vector space
- only has to satisfy closure under addition and multiplication