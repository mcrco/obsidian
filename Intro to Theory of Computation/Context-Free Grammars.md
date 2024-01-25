- just as [[Finite Automata]] recognize **regular languages** (languages described by [[Regular Expression]]),
- [[Pushdown Automata|NPDA]] recognizes **context-free languages** described by context-free grammars
- how it works?

![[Pasted image 20240122195517.png]]

- generate strings by repeated replacement of **non-terminals** with string of **terminals** and **non-terminals**
	- write start symbol (non-terminal)
	- replace non-terminal with RHS of a rule/production that has a non-terminal as its LHS
	- repeat above until no more non-terminals

# Examples

- given 
	- start symbol: $A$
	- productions: $A\to 0A 1$, $A\to B$, $B\to \#$
- $A\implies 0A 1 \implies 00A 11 \implies 000 A 111 \implies 000 B 111 \implies 000 \# 111$
- above is **derivation** for the string $000 \# 111$
- set of all strings generated this way: **language of the grammar** $L(G)$
- aka **context-free language**
- other examples: 
	- natural language (kinda)
	- computer language (often)

# Formal Definition

> [!math|{"type":"definition","number":"auto","setAsNoteMathLink":false,"title":"Context Free Grammar","label":"context-free-grammar","_index":0}] Definition 1 (Context Free Grammar).
> CFG is a 4-tuple 
> $$
> (V,\Sigma,R,S)
> $$
> where 
> - $V$: finite [[Sets|set]] of non-terminals
> - $\Sigma$: finite set ([[Sets#Intersection|disjoint]] from $V$) called terminals
> - $R$: finite set of **productions**, each production is non-terminal and string of terminals and non-terminals
> - $S \in V$: **start variable** or start non-terminal

- if $u,v,w$ are strings of non-terminals and terminals, and $A\to w$ is a production:
- $uAv$ yields $uwv$: $uAv \implies uwv$
- yields in $k$ steps: $u \overset{k}{\implies} \,v$
- $u \overset{*}{\implies}v$: $\exists k\geq 0$ and strings $u_{1},\dots,u_{k-1}$ for which $u\implies u_{1} \implies \dots \implies v$
- another definition of $L(G)$: $\{ w \in \Sigma^{\star}: S \overset{*}{\implies} w \}$ where $S$ is starting symbol

# Properties

- closed under 
	- union
	- concatenation
	- star
- every [[Regular Expression|regular language]] is a CFL

# NPDA CFG Equivalence

> [!math|{"type":"theorem","number":"auto","setAsNoteMathLink":false,"title":"NPDA CFG Equivalence","label":"npda-cfg-equivalence","_index":1}] Theorem 2 (NPDA CFG Equivalence).
> A language $L$ is recognized by a NPDA **iff** $L$ is described by CFG.

## Proof

`\begin{proof}` Must prove 2 directions:

1. ($\implies$) $L$ is recognized by NPDA $\implies$ $L$ is described by CFG
2. $(\impliedby)$ $L$ is described by CFG $\implies$ $L$ is recognized by NPDA

### Proof of $\impliedby$ 

- $L$ is described by CFG $\implies$ $L$ is recognized by a NPDA
- we want to non-deterministically guess derivation and form it on the stack
- then scan input, pop matching symbol from stack every step
- accept input if we get to bottom of stack at end of input



`\end{proof}`