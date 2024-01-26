# Span

> [!definition] Linear Combination
> %% label: linear-combination %%
> A vector of the form
> $$
> \sum_{i=1}^{n}a_{i}\cdot \vec{v_{i}}
> $$
> where $\vec{v_{i}} \in$ some vector space $V$ over $\mathbb{F}$ and $a_{i} \in \mathbb{F}$.

> [!definition] Span
> %% label: span %%
> For $K$-[[Vector Spaces|vector space]] $V$, $S=\{ v_{1},v_{2},\dots,v_{n} \} \subset V$, $\text{span}(S)=\{ a_{1}\vec{v}_{1} + \dots + a_{n}\vec{v}_{n} \}$ (set of all linear combinations). $S$ spans $V$ (or generates $V$) if $\text{span}(S)=V$ aka .

> [!definition] Finite Dimensional
> %% label: finite-dimensional %%
> A [[Vector Spaces|vector space]] is finite dimensional if finite set of vectors spans it.

- example: $\mathbb{R}^{2}$ is finite dimensional
- $\vec{u} \in \mathbb{R}^{2} =a\vec{v}_{1} + b\vec{v}_{2}$ for $a,b \in \mathbb{R}$ if $\vec{v_{1}}, \vec{v_{2}}$ are not on the same line through $(0,0)$ 
- this property of $\{ \vec{v_{1}},\vec{v_{2}} \}$ is called

# Linear Independence

> [!definition] Linear Independence
> %% label: linear-independence %%
> Given a set $S \subset V$, $S$ is linearly independent if given $a_{1}\vec{v_{1}}+\dots+a_{n}\vec{v_{n}}=\vec{0}$ with $a_{i} \in K$ and $\vec{v_{i}} \in S$ distinct, then $a_{1}=a_{2}=\dots=a_{n}=0$. 

> [!theorem]
> If $S$ is linearly independent then $T \subset S$ is linearly independent.

- opposite would be

> [!definition] Linear Dependence
> %% label: linear-dependence %%
> $S$ is linearly dependent if for $a_{1},\dots, a_{k} \in K$, $\vec{v_{1}},\dots,\vec{v_{n}} \in S$, $a_{1}\vec{v_{1}}+\dots+a_{n}\vec{v_{n}}=\vec{0}$ w/ some $a_{i}\neq 0$.

# Bases

> [!definition] Basis
> %% label: basis %%
> Basis of $V$ ($\mathcal{B}(V)$) is a list of vectors that is linearly independent and spans $V$.

^c71fc8

> [!proposition] Basis
> %% label: basis %%
> $S \subset V$ is a basis $\iff$ every vector $\vec{v} \in V$ can be expressed uniquely as $\vec{v} = a_{1}\vec{v_{1}} + \dots + a_{n}\vec{v_{n}}$.

`\begin{proof}`
$\impliedby$: definition of span
$\implies$: for $\vec{v}=a_{1}\vec{v_{1}}+\dots+a_{n}\vec{v_{n}}$ and $\vec{w}=b_{1}\vec{v_{1}}+b_{n}\vec{v_{n}}$,  $\vec{v}=\vec{w}\implies \vec{v}-\vec{w}=\vec{0}\implies (a_{1}-b_{1})\vec{v_{1}} + \dots + (a_{n}-b_{n})\vec{v_{n}} \implies a=b$
`\end{proof}`

> [!example] Standard Basis
> %% label: standard-basis %%
> $V=K^{n}$ has a standard basis $S=\{ e_{1},\dots,e_{n} \}$:
> $\vec{e_{1}}=(1,0,\dots,0)$
> $\vec{e_{2}}=(0,1,\dots,0)$
> ...
> $\vec{e_{n}}=(0,0,\dots,1)$

- example: a polynomial of degree $\leq d$ has standard basis $\{ 1,x,x^{2},\dots,x^{d} \}$

## Dimension

> [!definition] Dimension
> %% label: dimension %%
> If $V$ is basis $S$, **dimension** of $V$, or $\text{dim}(V)$ is $|S|$

> [!claim]
> $\text{dim}$ is well defined: any two bases of a finite dimensional vector space have same length.

`\begin{proof}`Suppose $S,T$ are bases. Then, if $S$ is linearly independent and $T$i s spanning,

$$
|S|\leq|T|.
$$

Since we can flip around WLOG, 

$$
|T|\leq|S|.
$$

Thus, $|S|=|T|$.
`\end{proof}`

# Connection to [[Sets]]

| Set Theory                                                                                                  | Linear Algebra                                                                               |
| ----------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------- |
| $A$ is a finite set                                                                                         | $V$ is finite dimensional                                                                    |
| $A$                                                                                                         | $\text{dim}(V)$                                                                              |
| $A_{1} \cup A_{2}$                                                                                          | $V_{1} + V_{2}$                                                                              |
| $\lvert A_{1} \cup A_{2} \rvert = \lvert A_1 \rvert + \lvert A_{2} \rvert - \lvert A_{1} \cap A_{2} \rvert$ | $\text{dim}(V_{1}+V_{2})=\text{dim}(V_{1})+\text{dim}(V_{2}) - \text{dim}(V_{1} \cap V_{2})$ |
| $\lvert \bigcup_{i=1}^{n}A_{i} \rvert = \sum_{i=1}^{n}\lvert A_{i} \rvert \iff \text{disjoint}$             | $\text{dim}\left( \sum_{i=1}^{n}V_{i} \right)=\sum_{i=1}^{n}\text{dim}(V_{i}) \iff \text{direct sum}$                                                                                             |