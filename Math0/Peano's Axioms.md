# Question 1

Let $a,b,c \in \mathbb{N}$. Show that if $a+b=a+c$, then $b=c$.

## Proof

We will perform a proof by induction. Consider the statement $S(a)$ given by if $a+b=a+c$, then $b=c$ for $a,b,c \in \mathbb{N}$.

We will start by proving the base case, $S(0).$ Since $x+0=x$ for all $x \in \mathbb{N}$ by definition, we know that $0+b=b$ and $0+c=c$. Thus, $a+b=a+c\implies 0+b=0+c \implies b=c$. 

Now, we perform the inductive step. Assume that $S(k)$ is true for $k \in N, k\geq 0$. So, we assume that if $k+b=k+c$, then $b=c$. We will use this information to prove $S(k+1)$, which is if $(k+1)+b=(k+1)+c$, then $b=c$. 

We start with the commutative property:

$$
\begin{gather*}
(k+1)+b=k+b+1
\end{gather*}
$$

# Question 2

a. Show that $a+a=2\cdot a$.

## Proof

By the reflexivity axiom, if we prove $2\cdot a=a+a$, we prove $a+a=2\cdot a$.

By commutativity, we know that $2\cdot a=a\cdot{2}$. By the definition of multiplication, we know that $a\cdot 2= a\cdot S(1)=a+(a\cdot 1)=a+(a\cdot S(0))=a+(a+(a\cdot 0))=a+a+0=a+a.$ 
Since we have proved $a\cdot 2=2\cdot a=a+a$, we have proven $a+a=2\cdot a$.

b. Show that $a+a+a\dots+a=n\cdot a$.

## Proof

Once again, we can prove the statement by proving the reflected statement with a commutated product: $a\cdot n=a+a\dots+a$. We will do a proof by induction. Consider the statement $S(n)$ given by $a\cdot n=a+a+\dots+a$ $n$ times for $n\geq 0$. 

The base case, $S(0)$, is given by $a\cdot 0=0$. This is true by the definition of multiplication.

Now, we perform the inductive step. Assume that $S(k)$ is true for $k\geq 0$. Thus,

$$
a\cdot k=a+a+\dots+a
$$

$k$ times. We will use this to prove $S(k+1):$

$$
a\cdot(k+1)=a+a+\dots+a
$$

$k+1$ times. 

Starting with the LHS of $S(k+1)$, we use the distributive property to get

$$
\begin{align*}
a\cdot(k+1)&=a\cdot k+a\cdot 1 \\
&= a\cdot k+a\cdot S(0) \\
&= a\cdot k+a+a\cdot 0 \\
&= a\cdot k+a.
\end{align*}
$$

Since we know that $a\cdot k=a+a+\dots+a$ $k$ times, $a\cdot k+a = a+a+\dots+a$ $k+1$ times. Thus, we have proven that $S(k+1)$ is true.

By mathematical induction, we have proven the statement $S(n)$ given by $a\cdot n=a+a+\dots+a$ $n$ times, and thus, we have proven $a+a\dots+a$ $n$ times equals $n\cdot a$.

# Question 3

a. Let $a,b,c \in N$ such that $c\neq 0$ and $a=b\cdot c$. Prove that $b\leq a$. 

By the definition of multiplication, we get that $b\cdot c=b + b\cdot S^{-1}(c)$.  Since we know that $c\neq 0$ and $c \in \mathbb{N}$, $S^{-1}(c) \in \mathbb{N}$. Thus, $a=b+b\cdot S^{-1}(c)$ for $a,b,S^{-1}(c) \in \mathbb{N}$., We know that $b \cdot S^{-1}(c)\geq 0$ because the smallest possible result of a multiplication between 2 natural numbers is $0.$ Therefore, $a\geq b$ and $b\leq a$.

b. 