- [[Finite Dimensional Vector Spaces#Connection to Sets|vector spaces]]  $\iff$ [[Sets|sets]] and  
- [[Linear Maps|linear maps]]  $\iff$ [[Functions|functions]]
- how do these "functions" apply to "sets"?

# Kernel

> [!definition] Kernel
> %% label: kernel %%
> The **kernel** of a [[Linear Maps|linear map]] $T \in \mathcal{L}(V,W)$ is the set of all vectors in $V$ that map to $0$.
> $$
> \text{ker}T = \{ v|T(v)=0 \}
> $$

## Examples

- kernel of zero map is entire space
- kernel of differentiation map is constant functions
- kernel of squared map is $\{ 0 \}$

## Relation to $V$

> [!claim]
> For any $T \in \mathcal{L}(V,W)$, $\mathrm{ker}T$ is a subspace of $V$.

`\begin{proof}`$0 \in \text{ker }T$ for obvious reasons:

$$
T(0)=T(0+0)=T(0)+T(0)\implies T(0)=0
$$

`\end{proof}`