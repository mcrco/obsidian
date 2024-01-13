# Span

> [!math|{"type":"definition","number":"auto","setAsNoteMathLink":false,"title":"Span","label":"span","_index":0}] Definition 1 (Span).
> For $K$-[[Vector Spaces|vector space]] $V$, $S=\{ v_{1},v_{2},\dots,v_{n} \} \subset V$, $\text{span}(S)=\{ a_{1}\vec{v}_{1} + \dots + a_{n}\vec{v}_{n} \}$. $S$ spans $V$ (or generates $V$) if $\text{span}(S)=V$.

- example: any vector $\vec{u} \in \mathbb{R}^{2} =a\vec{v}_{1} + b\vec{v}_{2}$ if $\vec{v_{1}}, \vec{v_{2}}$ are not on the same line through $(0,0)$. 
- this property of $\{ \vec{v_{1}},\vec{v_{2}} \}$ is called

> [!math|{"type":"definition","number":"auto","setAsNoteMathLink":false,"title":"Linear Independence","label":"linear-independence","_index":1}] Definition 2 (Linear Independence).
> Given a set $S \subset V$, $S$ is linearly independent if given $a_{1}\vec{v_{1}}+\dots+a_{n}\vec{v_{n}}=\vec{0}$ with $a_{i} \in K$ and $\vec{v_{i}} \in S$ distinct, then $a_{1}=a_{2}=\dots=a_{n}=0$. 

> [!math|{"type":"theorem","number":"auto","setAsNoteMathLink":false,"_index":2}] Theorem 3.
> If $S$ is linearly independent then $T \subset S$ is linearly independent.

- opposite would be

> [!math|{"type":"definition","number":"auto","setAsNoteMathLink":false,"title":"Linear Dependence","label":"linear-dependence","_index":3}] Definition 4 (Linear Dependence).
> $S$ is linearly dependent if for $a_{1},\dots, a_{k} \in K$, $\vec{v_{1}},\dots,\vec{v_{n}} \in S$, $a_{1}\vec{v_{1}}+\dots+a_{n}\vec{v_{n}}=\vec{0}$ w/ some $a_{i}\neq 0$.

# Basis

> [!math|{"type":"proposition","number":"auto","setAsNoteMathLink":false,"title":"Basis","label":"basis","_index":4}] Proposition 5 (Basis).
> $S \subset V$ is a basis $\iff$ every vector $\vec{v} \in V$ can be expressed uniquely as $\vec{v} = a_{1}\vec{v_{1}} + \dots + a_{n}\vec{v_{n}}$.

`\begin{proof}`
$\impliedby$: definition of span
$\implies$: for $\vec{v}=a_{1}\vec{v_{1}}+\dots+a_{n}\vec{v_{n}}$ and $\vec{w}=b_{1}\vec{v_{1}}+b_{n}\vec{v_{n}}$,  $\vec{v}=\vec{w}\implies \vec{v}-\vec{w}=\vec{0}\implies (a_{1}-b_{1})\vec{v_{1}} + \dots + (a_{n}-b_{n})\vec{v_{n}} \implies a=b$
`\end{proof}`

> [!math|{"type":"example","number":"auto","setAsNoteMathLink":false,"title":"Standard Basis","label":"standard-basis","_index":5}] Example 6 (Standard Basis).
> $V=K^{n}$ has a standard basis $S=\{ e_{1},\dots,e_{n} \}$:
> $\vec{e_{1}}=(1,0,\dots,0)$
> $\vec{e_{2}}=(0,1,\dots,0)$
> ...
> $\vec{e_{n}}=(0,0,\dots,1)$

- example: a polynomial of degree $\leq d$ has standard basis $\{ 1,x,x^{2},\dots,x^{d} \}$

> [!math|{"type":"definition","number":"auto","setAsNoteMathLink":false,"title":"Dimension","label":"dimension","_index":6}] Definition 7 (Dimension).
> If $V$ is basis $S$, **dimension** of $V$, or $\text{dim}(V)$ is $|S|$

> [!math|{"type":"claim","number":"auto","setAsNoteMathLink":false,"_index":7}] Claim 8.
> $\text{dim}$ is well defined

`\begin{proof}`Suppose $S,T$ are bases, $|S|<|T|$. 
`\end{proof}`