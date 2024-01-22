- [[Finite Dimensional Vector Spaces#Connection to Sets|vector spaces]]  $\iff$ [[Sets|sets]] and  
- [[Linear Maps|linear maps]]  $\iff$ [[Functions|functions]]
- how do these "functions" apply to "sets"?

# Kernel

> [!math|{"type":"definition","number":"auto","setAsNoteMathLink":false,"title":"Kernel","label":"kernel","_index":0}] Definition 1 (Kernel).
> The **kernel** of a [[Linear Maps|linear map]] $T \in \mathcal{L}(V,W)$ is the set of all vectors in $V$ that map to $0$.
> $$
> \text{ker}T = \{ v|T(v)=0 \}
> $$

## Examples

- kernel of zero map is entire space
- kernel of differentiation map is constant functions
- kernel of squared map is $\{ 0 \}$

## Relation to $V$

> [!math|{"type":"claim","number":"auto","setAsNoteMathLink":false,"_index":1}] Claim 2.
> For any $T \in \mathcal{L}(V,W)$, $\mathrm{ker}T$ is a subspace of $V$.

`\begin{proof}`$0 \in \text{ker }T$ for obvious reasons:

$$
T(0)=T(0+0)=T(0)+T(0)\implies T(0)=0
$$

`\end{proof}`