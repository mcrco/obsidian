# Problem

> [!definition] Problem
> %% label: problem %%
> A problem associates each input to an output. Input and output are strings over a finite alphabet $\Sigma^{}$. $\Sigma^{\star}$ is infinite [[Sets|set]] of finite strings.
> 
> $$
> f:\Sigma ^{\star} \to \Sigma^{\star}
> $$

More simply,

> [!definition] Decision Problem
> %% label: decision-problem %%
> $f:\Sigma^{\star} \to \{ \text{accept}, \text{reject} \}$

**Every problem has a simpler decision problem**.

## Prime Factoring

Given an integer $m$, find its prime factors. Integers are represented as $\{ 0,1 \}^{\star}$ cuz binary.

### Problem

$$
f_{\text{factor}}:\{ 0,1 \}^{\star}\to \{ 0,1 \}^{\star}.
$$

$f_{\text{factor}}$ outputs [[Sets|set]] of prime factors.

### Decision

$$
f:\{ m,k \}\to \{ \text{accept}, \text{reject} \}.
$$

$f$ outputs whether or not $m$ has a prime factor smaller than $k$. Can be paired with binary search to solve original problem.

# Computation

> [!definition] Computation
> %% label: computation %%
> $$
> \text{input} \to \text{machine} \to \begin{cases}
> \text{accept} \\
> \text{reject} \\
> \text{loop forever}
> \end{cases}
> $$

> [!definition] Language
> %% label: language %%
> $L \subseteq \Sigma^{\star}$: subset of strings over $\Sigma^{}$

^3dcd80

> [!definition] Recognition
> %% label: recognition %%
> [[Sets|set]] of strings that lead to accept is language **recognized** by machine

> [!definition] Decision
> %% label: decision %%
> every other string ($x \notin L$) leads to reject $\implies$ language is **decided** by the machine