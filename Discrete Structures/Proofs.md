All reasoning is based on assumptions, called **axioms** and **postulates**, and definitions. 

Sometimes we have undefined terms: ideas we agree on but can't prove. 

# Proven Statements

- theorem: a truth established through a proof
- lemma: proven statement used in proof of theorem
- corollary: proven statement easily derived from theorem

# Counterexamples

A counterexample is a way to disprove a statement by giving an instance where the statement is false.

# Types of Proofs

## Direct Proofs

- most often
- start and beginning, progress to end
- "makes sense"
- often very hard

### Example Direct Proofs

#### Preliminary Ideas:

1. Definition of even and odd
2. $x > y, \, z > t \implies x + z > y + t$ 
3. $a > 0,\, b > 0 \implies ab > 0$
4. $x > y > 0, \, z > t > 0 \implies xz > yt$ 
5. The sum, difference, and product of integers is another integer

#### Proof 1

##### Claim

If a > 0, b > 0, a > b, then $a^{2} > b^{2}$.

##### Lemma

If $x > 0$, $y > 0$, then $x + y > 0$

###### Proof of Lemma

By PI2:

$$
x > y, z > t \implies x + z > y + t \implies a + b > 0
$$

##### Proof of Claim 

$$
a > b \implies a - b > 0
$$

Combining the above equation with the lemma, we use PI3 to get:

$$
\begin{align}
(a + b)(a - b) &> 0 \cdot 0 \\
a^{2} - b^{2} &> 0 \\
a^{2} &> b^{2}
\end{align}
$$

#### Proof 2

##### Claim

If $n$ is odd, then $n^{2}$ is odd.

##### Proof of Claim 

$n$ is odd. By PI1,

$$
n = 2k + 1
$$

for some integer $k$.

Then 

$$
\begin{align}
n^{2} = (2k + 1)^{2} &= 4k^{2} + 4k + 1 \\
&= 2(2k^{2} + 2k) + 1 \\
\end{align}
$$

By PI5 (multiple times) and PI1, we get that $n^{2}$ is odd number as well.

## Indirect Proofs

- used when direct proof isn't possible
- starts by assuming our claim is false
- derive a contradiction
- also called **proof by contradiction**

### Example Proofs

#### Proof 1

##### Claim

If $n^{2}$ is even, then $n$ is even.

##### Lemma

Our previous proof for $n^{2}$ is odd if $n$ is odd will come in handy.

##### Indirect Proof of Claim

Assume $n^{2}$ is even, but $n$ is odd.

By our lemma, $n^{2}$ should then be odd, but that contradicts our assumption. 