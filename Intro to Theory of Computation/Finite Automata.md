# Finite Automata

- simple model of computation
- reads input left to right, one symbol at a time
- maintains **state**
	- information about seen inputs
	- finite automaton $\implies$ finite # of states (loses memory over time)
- described by diagram or formally

## Diagram

![[Pasted image 20240105131038.png]]

- start arrow at left
- alphabet in example: $\{ 0,1 \}$
- states: $q_{1},q_{2},q_{3}$
	- $q_{3}$ is accept state
- transitions are arrows denoted by number (input)
- this FA decides $L=\{ x:x \in \{ 0,1 \}^{\star},x_{n-1}=1 \land x_{n}=0 \}$
	- language is every string ending with $10$

## Formal Definition

> [!math|{"type":"definition","number":"auto","setAsNoteMathLink":false,"title":"Finite Automaton","label":"finite-automaton","_index":0}] Definition 1 (Finite Automaton).
> A finite automaton is a 5-tuple
> $$
> \left( Q,\Sigma, \sigma, q_{0}, F \right)
> $$
> - $Q$: finite set called the states
> - $\Sigma$: finite set called the alphabet
> - $\sigma$: [[Single Variable Calculus/Functions|function]] $Q\times\Sigma\to Q$ called transition function
> - $q_{0}$: start state
> - $F$: subset of $Q$ containing accept states

^02be7c

## FA Languages

- union "$C=A \cup B$"
	- [[Sets|set]] of languages recognized by FA is closed under union
- concatenation "$C=A\circ B$"
	- $A\circ B=\{ xy:x \in A \land y\in B \}$
	- how to concatenate?
		- can try turning accept states of $A$ into start states of $B$
		- but then FA might start parsing string for $B$ when it should still be parsing $A$
		- need free transition $\epsilon$
		- multiple transitions with same label?!
		- introduces non-determinism, creating

## Non-Deterministic Finite Automaton

- can think of NFA operation as
- $x$ is accepted if //INSERT

> [!math|{"type":"definition","number":"auto","setAsNoteMathLink":false,"title":"Nondeterministic Finite Automaton","label":"nondeterministic-finite-automaton","_index":1}] Definition 2 (Nondeterministic Finite Automaton).
> $$
> (Q,\Sigma,\sigma,q_{0},F)
>$$
>- $Q,\Sigma,q_{0},F$ are same as [[#^02be7c]] 
>- $\sigma$

> [!math|{"type":"definition","number":"auto","setAsNoteMathLink":false,"title":"NFA Operation","label":"nfa-operation","_index":2}] Definition 3 (NFA Operation).
> NFA $M$ accepts a string $w=w_{1}w_{2}w_{3}\dots w_{n} \in \Sigma^{\star}$ if