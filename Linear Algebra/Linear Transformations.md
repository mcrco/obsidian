- we can move from one [[Vector Spaces|vector space]] to another by a 

> [!math|{"type":"definition","number":"auto","setAsNoteMathLink":false,"title":"Linear Map","label":"linear-map","_index":0}] Definition 1 (Linear Map).
> A **linear map** from $V$ to $W$ is a function $T:V\to W$ s.t. it obeys
> - additivity: $T(u+v)=T(u)+T(v)$ for all $u,v \in V$
> - homogeneity: $T(\lambda u)=\lambda T(u)$ for all $u \in V$, $\lambda \in \mathbb{F}$

- $\mathcal{L}(V,W)$ is set of all linear maps from $V \to W$
	- $\mathcal{L}(V)=\mathcal{L}(V,V)$
- just as [[Finite Dimensional Vector Spaces#Connection to Sets|vector space $\iff$ sets]], linear maps $\iff$ functions

# Examples

- zero map $\mathbf{0} \in \mathcal{L}(V,W)$ maps every element in $V$ to zero element of $W$ ($\mathbf{0}_{W}$)
- identity map $I \in \mathcal{L}(V)$ maps every element of $V$ to itself
-  "squared" map $T \in \mathcal{L}(\mathcal{P}(\mathbb{F}))$ multiplies every polynomial by $x^{2}$
- differentiation map $D \in \mathcal{L}(\mathcal{P}(\mathbb{F}))$ takes derivative of a polynomial
	- $D(p(x))=p'(x)$ for $p(x) \in \mathcal{P}(\mathbb{F})$
- integration map $E \in \mathcal{L}(\mathcal{P}(\mathbb{F}),\mathbb{R})$ computes integral on $[0,1]$

# Linear Maps as [[Vector Spaces]]

> [!math|{"type":"theorem","number":"auto","setAsNoteMathLink":false,"_index":1}] Theorem 2.
> Suppose $\{ v_{1},\dots,v_n \}$ is a basis of $V$ and $\{ w_{1},\dots,w_{n} \}$ is a basis of $W$. There **exists** a **unique** linear map s.t. the following is true for $k=1,2,\dots,n$
> $$
> Tv_{k}=w_{k}
> $$

^4eeb4a

`\begin{proof}`
TODO
`\end{proof}`

- [[#^4eeb4a]]'s **existence** condition $\implies$ linear map can map any basis vector of $V$
- **unique** condition $\implies$ fixing basis of $V$ that maps to a basis in $W$ $\implies$ $T$ is determined for $V$
- can use this to claim

> [!math|{"type":"claim","number":"auto","setAsNoteMathLink":false,"_index":2}] Claim 3.
> $\mathcal{L}(V,W)$ is a [[Vector Spaces|vector space]].

- by defining

> [!math|{"type":"definition","number":"auto","setAsNoteMathLink":false,"_index":3}] Definition 4.
> For $S,T \in \mathcal{L}(V,W)$, we define operations on maps as follows for $v \in V$
> - **addition**: $(S+T)(v) = S(v) + T(V)$
> - **scalar multiplication**: $(\lambda S)(v)=\lambda\cdot S(v)$

- composition for $T \in \mathcal{L}(V,U)$, $S \in \mathcal{L}(U,W)$ defined as

$$
(ST)(v)=S(T(v))
$$

- not commutative