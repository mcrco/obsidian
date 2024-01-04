# Definition

> [!math|{"type":"definition","number":"auto","setAsNoteMathLink":false,"title":"Problem","label":"problem","_index":0}] Definition 1 (Problem).
> A problem associates each input to an output. Input and output are strings over a finite alphabet $\sum_{}^{}$. $\sum_{}^{\star}$ is infinite set of finite strings.
> 
> $$
> f:\sum ^{\star} \to \sum^{\star}
> $$

More simply,

> [!math|{"type":"definition","number":"auto","setAsNoteMathLink":false,"title":"Decision Problem","label":"decision-problem","_index":1}] Definition 2 (Decision Problem).
> $f:\sum_{}^{\star} \to \{ \text{accept}, \text{reject} \}$

**Every problem has a simpler decision problem**.

## Prime Factoring

Given an integer $m$, find its prime factors. Integers are represented as $\{ 0,1 \}^{\star}$ cuz binary.

### Problem

$$
f_{\text{factor}}:\{ 0,1 \}^{\star}\to \{ 0,1 \}^{\star}.
$$

$f_{\text{factor}}$ outputs set of prime factors.

### Decision

$$
f:\{ m,k \}\to \{ \text{accept}, \text{reject} \}.
$$

$f$ outputs whether or not $m$ has a prime factor smaller than $k$. Can be paired with binary search to solve original problem.

# Computation

> [!math|{"type":"definition","number":"auto","setAsNoteMathLink":false,"title":"Computation","label":"computation","_index":2}] Definition 3 (Computation).
> $$
> \text{input} \to \text{machine} \to \begin{cases}
> \text{accept} \\
> \text{reject} \\
> \text{loop forever}
> \end{cases}
> $$

- **language** $L \subset \sum_{}^{\star}$: subset of strings over $\sum_{}^{}$
- set of strings that lead to accept is language **recognized** by machine
- every other string leads to reject $\implies$ language is **decided** by the machine