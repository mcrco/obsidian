- [[Finite Automata]] are limited by lack of memory with bounded information
- how to change so FA can recognize languages like $\{ 0^{n}1^{n}:n\geq 0 \}$?
- add an (infinite) stack that we can push and pop from

![[Pasted image 20240122104623.png]]

> [!math|{"type":"definition","number":"auto","setAsNoteMathLink":false,"title":"Non-deterministic Pushdown Automaton","label":"non-deterministic-pushdown-automaton","_index":0}] Definition 1 (Non-deterministic Pushdown Automaton).
> NPDA $M=(Q,\Sigma,\Gamma,\delta,q_{0},F)$ 
>
>- $Q$: finite set of states
>- $\Sigma$: finite set of tape alphabet
>- $\Gamma$: finite set of stack alphabet
>- $\delta$: $Q\times (\Sigma \cup \{ \epsilon \}) \times (\Gamma \cup \{ \epsilon \}) \to \mathcal{P}(Q \times (\Gamma \cup \{ \epsilon \}))$ is transition function
>	- $\delta(a,b\to c)$: 
>		- read $a$ from stack if not $\epsilon$
>		- pop $b$ from stack if not $\epsilon$
>		- push c onto stack if not $\epsilon$
>		- go to next state with new stack (or top element of stack as defined above)
>- $q_{0}$: start state
>- $F$: accept states

- **same shit but in English:**
- basically a NPDA is [[Finite Automata]] but you pair it with a stack
- whenever you read in a new character (symbol), say $a$, from string (tape), you find a transition with the first parameter being $a$
- whatever comes after the comma is popped from the stack (pop nothing if transition is of the form $a,\epsilon \to \text{symbol}$)
- the symbol on the other side of the arrow is pushed onto stack
- go to the next state

> [!math|{"type":"definition","number":"auto","setAsNoteMathLink":false,"title":"NPDA Acceptance","label":"npda-acceptance","_index":1}] Definition 2 (NPDA Acceptance).
> NPDA accepts string $w=\Sigma^{\star}$ if $w$ can be written as
> $$
> w_{1}w_{2}w_{3}\dots w_{m}\in(\Sigma \cup \{ \epsilon \})^{\star}
> $$
> and 
> - there exists states $r_{0},r_{1},\dots ,r_{m}$ and 
> - there exists strings $s_{0},s_{1},\dots ,s_{m}$ in $(\Gamma \cup \{ \epsilon \})^{\star}$
> 	- $r_{0}=q_{0}$ and $s_{0}=\epsilon$
> 	- $(r_{i+1},b) \in \delta(r_{i},w_{i+1},a)$ where $s_{i}=at,s_{i+1}=bt$ for some $t \in \Gamma$
> 	- $r_{m} \in F$

- **same shit but in English**:
- 

# Context-Free Grammars

- just as [[Finite Automata]] recognize **regular languages** (languages described by [[Regular Expression]]),
- NPDA recognizes **context-free languages** described by [[Context-Free Grammars]]