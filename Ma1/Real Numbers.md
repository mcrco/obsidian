- set of infinite decimal expansions
- $a_{0}.a_{1}a_{2}a_{3}\dots$, where $a_{0}\in\mathbb{Z}$ and $0\leq a_{i}\leq 9$ for $i\geq 1$.
- 'fills in number line'
- $0.\bar{9} = 1$

# Field Axioms

On $\mathbb{R}$, there are 2 binary operations $+$ and $\cdot$ such that 

> [!math|{"type":"axiom","number":"auto","setAsNoteMathLink":false,"title":"Commutativity","label":"commutativity","_index":0}] Axiom 1 (Commutativity).
> $x=y=y+x$, $xy = yx$.

> [!math|{"type":"axiom","number":"auto","setAsNoteMathLink":false,"title":"Associativity","label":"associativity","_index":1}] Axiom 2 (Associativity).
> $$
> \begin{gather*}
> x+(y+z)\geq(x+y)+z, \\
> x(yz) = (xy)z \\
> \end{gather*}
> $$ 

> [!math|{"type":"axiom","number":"auto","setAsNoteMathLink":false,"title":"Distributivity","label":"distributivity","_index":2}] Axiom 3 (Distributivity).
> $$
>x(y+z)=xy+xz
>$$

> [!math|{"type":"axiom","number":"auto","setAsNoteMathLink":false,"title":"Existence of $0,1$","label":"existence-of-01","_index":3}] Axiom 4 (Existence of $0,1$).
> $$
> \begin{gather}
> 0+x=0,  \\
> 1\cdot x=x \\
> \end{gather}
> $$

> [!math|{"type":"axiom","number":"auto","setAsNoteMathLink":false,"title":"Existence of Negatives","label":"existence-of-negatives","_index":4}] Axiom 5 (Existence of Negatives).
> $$
> \forall x, \exists y\mid y+x=0
> $$
> $y$ is the definition of $-x$.

> [!math|{"type":"axiom","number":"auto","setAsNoteMathLink":false,"title":"Existence of Reciprocals","label":"existence-of-reciprocals","_index":5}] Axiom 6 (Existence of Reciprocals).
> $$
> \forall x, \exists y\mid yx=1
> $$

Any subset $F$ of $\mathbb{R}$ with these properties is called a field. Example: $\mathbb{Q}$, the set of rationals.

> [!math|{"type":"lemma","number":"auto","setAsNoteMathLink":false,"title":"Cancellation","label":"cancellation","_index":6}] Lemma 7 (Cancellation).
> If $a+b=a+c$, then $b=c$
> `\begin{proof}`
> By [[#^d0c340]] , $\exists y \mid y+a=0$. Therefore, if $a+b=a+c$, we can add $y$ on both sides to get 
> 
> $$
> y+(a+b) = y+(a+c).
> $$
>
By [[#^8fd086]] , we get 
>
>$$
>\begin{align}
>(y+a)+b&=y+a)+c  \\
>0+b&=0+c
>\end{align}
>
>$$
>
> By [[#^2f82da]] , we get
>
>$$
>b=c
>$$
> `\end{proof}`

^cb5aca

> [!math|{"type":"lemma","number":"auto","setAsNoteMathLink":false,"_index":7}] Lemma 8.
> $(-1)(-1)=1$

`\begin{proof}`
`\end{proof}`
# Order Axioms

There is a subset $\mathbb{R}_{+}$ of $\mathbb{R}$ such that 

> [!math|{"type":"axiom","number":"auto","setAsNoteMathLink":false,"title":"Closure Under Addition","label":"closure-under-addition","_index":8}] Axiom 9 (Closure Under Addition).
> $$
> x,y \in \mathbb{R}_{+} \implies x+y, xy \in \mathbb{R}_{+}
> $$

^895ad9

> [!math|{"type":"axiom","number":"auto","setAsNoteMathLink":false,"_index":9}] Axiom 10.
> If $x \neq 0$, then either $x \in \mathbb{R}_{+}$ or $x \in \mathbb{R}_{+}$, but not both.

> [!math|{"type":"axiom","number":"auto","setAsNoteMathLink":false,"_index":10}] Axiom 11.
> $$
> 0 \not\in\mathbb{R}.
> $$

We may now define

> [!math|{"type":"definition","number":"auto","setAsNoteMathLink":false,"title":"Comparator","label":"comparator","_index":11}] Definition 12 (Comparator).
> 
> $$
> \begin{gather*}
> x<y \iff y - x \in \mathbb{R}_{+} \\
> x>y \iff y<x \iff x-y \in \mathbb{R}_{+}
> \end{gather*}
> $$
In particular, $x>0$ iff $x \in \mathbb{R}_{+}$.

> [!math|{"type":"lemma","number":"auto","setAsNoteMathLink":false,"title":"Transitivity of Comparator","label":"transitivity-of-comparator","_index":12}] Lemma 13 (Transitivity of Comparator).
> If $a<b$ and $b<c$, then $a<c$. 
> `\begin{proof}`
> $a<b$ and $b<c$ mean that $b-a\in \mathbb{R}_{+}$ and $c-b\in\mathbb{R}_{+}$.
> 
> But, by [[#^895ad9]], 
> 
> $$
> \begin{gather}
> (c-b)+(b-a) \in \mathbb{R}_{+} \\
> \implies c-a \in \mathbb{R}_{+} \\
> \implies a < c
> \end{gather}
> $$
> `\end{proof}`

> [!math|{"type":"lemma","number":"auto","setAsNoteMathLink":false,"_index":13}] Lemma 14.
> If $a<b$ and $c>0$, then $ac<b$.
> `\begin{proof}`
> $b-a>0$ and $c>0$ implies by 7 that $(b-a)c>0 \implies bc-ac>0 \implies ac<bc$.
> `\end{proof}`

> [!math|{"type":"lemma","number":"auto","setAsNoteMathLink":false,"_index":14}] Lemma 15.
> $$
> a\neq 0\implies a^{2}>0
> $$
> `\begin{proof}`
> If $a>0$, then $a^{2}>0$ by previous lemma. 
> 
> Assume $a^{2}\leq0$. Then, because $a\neq 0$, we must have $a<0$. However, that implies by axiom 8 that $-a>0 \implies (-a)^{2}>0 \implies a^{2}>0$, a contradiction.
> `\end{proof}`

# Def

Suppose $S$ is a nonempty subset of $\mathbb{R}$ and $B \in \mathbb{R}$ is such that $x\leq B$ for all $x \in S$. Then, we can say $B$ is an upperbound for $S$.

> If $B \in S$, we call B the maximum of $S$

# Def

$B \in \mathbb{R}$ is a least upper bound for a nonempty set $S$ if 

1. $B$ is an upperbound for $S$.
2. No number less than $B$ is an upperbound for $S$

> [!math|{"type":"theorem","number":"auto","setAsNoteMathLink":false,"title":"Unique upper bound","label":"unique-upper-bound","_index":15}] Theorem 16 (Unique upper bound).
> The least upper bound for a set $S$ is unique

`\begin{proof}`

`\end{proof}`

> [!math|{"type":"definition","number":"auto","setAsNoteMathLink":false,"title":"Supremum","label":"supremum","_index":16}] Definition 17 (Supremum).
> If it exists, the least upper bound of a set $S$ is called the supremum of $S$, denoted $\text{sup}(S)$. 
> Suppose  $x = a_{0}.a_{1}a_{2}a_{4}\dots$ where $\dots$
> 
> Let 

> [!math|{"type":"axiom","number":"auto","setAsNoteMathLink":false,"title":"Continuitiy Axiom","label":"continuitiy-axiom","_index":17}] Axiom 18 (Continuitiy Axiom).
> Every nonempty set of real numbers which is bounded above has a least upper bound or supremum
> `\begin{proof}`We can simply prove that $-S$ which is bonded below has a greatest lower bound or infimum`\end{proof}`

> [!math|{"type":"theorem","number":"auto","setAsNoteMathLink":false,"_index":18}] Theorem 19.
> The natural number $\mathbb{N}$ are unbounded above.
> `\begin{proof}`Suppose instead that $\mathbb{N}$ is bounded above. Then, by continuity axiom, it has a supremum $B$. So $B-1$ is not an upper bound, so there is some $n \in \mathbb{N} \mid n>B-1$. But then $n+1\in\mathbb{N}$ has $n+1>B$, contradicting that $B$ is an upper bound.`\end{proof}`

> [!math|{"type":"theorem","number":"auto","setAsNoteMathLink":false,"label":"archimedean-property","_index":19,"title":"Archimedean Property"}] Theorem 20 (Archimedean Property).
> If $x>0$ any $y\in\mathbb{R}$, $\exists n \mid nx>y$.
> `\begin{proof}`If not, then $\frac{y}{x}\geq n$ for all $n\in \mathbb{N}$, so $\mathbb{N}$ would be bounded above.`\end{proof}`

> [!math|{"type":"theorem","number":"auto","setAsNoteMathLink":false,"title":"\\sqrt{2}","label":"sqrt","_index":20}] Theorem 21 (\sqrt{2}).
> 2 has a positive square root.
> `\begin{proof}`Let $S=\{ x \in \mathbb{R} \mid x^{2}\leq 2 \}$. Consider $\text{sup}(S)$. We claim that $\text{sup}(S)^{2}=2$, so we need to disprove that $\text{sup}(S)^{2} > 2$ and $\text{sup}(S)^{2}<2$. But first, we need to show that $\text{sup}(S)$ exists. To see that $S$ is non-empty, note that $0^{2}\leq 2$. To see that $S$ is bounded above, note $2^{2}=4>2$. Thus, by Continuity Axiom, $\text{sup}(S)$ does exist.  
> Let $B=\text{sup}(S)$. 
> Case A: $B^{2}>2$.
> Let $C=\frac{1}{2}(B+\frac{2}{B})$. Then, $C<B$. We can prove this by starting with $\frac{1}{2}\left( B+\frac{2}{B} \right) < B \iff \frac{1}{B} < \frac{B}{2} \iff 2<B^{2}$. But also, $C^{2}=\frac{1}{4}(B^{2}+4+\frac{4}{B^{2}}=2+\dots>2$. Therefore, $C$ is a smaller upper bound for $S$, contradicting the definition of $B=\text{sup}(S)$.
> Case B: $B^{2} < 2$. 
> Choose $C\mid C<B$, $C < \frac{2-B^{2}}{3B}, C>0$. Then, $(B+C)^{2}=B^{2}+2BC+C^{2}$. That is $B^{2}+C(2B+C)<B^{2}+3BC<B^{2}+(2-B^{2})=2$, contradicting that $B=\text{sup}(S)$. 
> `\end{proof}`

# Sequence of Real Numbers

> [!math|{"type":"definition","number":"auto","setAsNoteMathLink":false,"title":"","label":"","_index":21}] Definition 22.
> A sequence of real numbers is a set
> $$
> a_{1},a_{2},a_{3}\dots
> $$
> of real numbers indexed by the natural numbers. Usually, we write $(a_{n})_{n=1}^{\infty}$ or $a_{n}$.

## Examples

$a_{n}=\frac{1}{n}$: we can see that $a_{n} \to 0$ as $n\to \infty$, We can say that $a_{n}$ is converging to the limit $0$.

$a_{n}=(-1)^{n} \implies (a_{n})_{n=1}^{\infty}=(-1, 1, -1, 1, \dots)$. This just oscillates and doesn't converge.

Now, if $a_{n}=\frac{(-1)^{n}}{n}=(-1, \frac{1}{2}, -\frac{1}{3}, \frac{1}{4},\dots$, this also converges to the limit $0$.

# Convergence

> [!math|{"type":"definition","number":"auto","setAsNoteMathLink":false,"title":"Convergence","label":"convergence","_index":22}] Definition 23 (Convergence).
> A sequence $(a_{n})^{\infty}_{n=1}$ converges to the limit $A$ iff for every $\forall \epsilon>0, \exists N=N(\epsilon): |a_{n}-A|<\epsilon , n\geq N$. We write $\lim_{ n \to \infty }a_{n}=A$.

## Examples

Show that $a_{n}=\frac{1}{n} \to 0$. 

`\begin{proof}` 

Fix $\epsilon>0$ and choose $N>\dots$.

Then, $\forall n\geq N$, we have

$$
| \frac{1}{n} - 0 | = \frac{1}{n} \leq \frac{1}{N} < \epsilon
$$
`\end{proof}`

> [!math|{"type":"lemma","number":"auto","setAsNoteMathLink":false,"_index":23}] Lemma 24.
> If $(a_{n})$ and $(b_{n})$ are sequences with $\lim_{ n \to \infty }a_{n}=A$ and $\lim_{ n \to \infty }b_{n}=B$, then 
> a. $\lim_{ n \to \infty }(a_{n}+b_{n})=A+B$
> `\begin{proof}`\Since $\lim_{ n \to \infty }a_{n}=A$, $\exists N\mid |a_{n_{1A|<}}-\frac{\epsilon}{2} \forall n_{1}\geq N_{1}$. If Since $\lim_{ n \to \infty }b_{n}=B$, $\exists N_{2} \mid |b_{n}-B|< \frac{\epsilon}{2}, \forall n_{2}\geq N_{2}$. 
> If we let $N=max(N_{1},N_{2})$, then $\forall n\geq N$, $|a_{n}+b_{n}-(A+B)| = |(a_{n}-A) + (b_{n}-B)$ $\leq |a_{n}-A| + |b_{n} - B| < \frac{\epsilon}{2} + \frac{\epsilon}{2} = \epsilon$.
> `\end{proof}`
> b. $\lim_{ n \to \infty }ca_{n}=cA$ for $c \in \mathbb{R}$
> c. $\lim_{ n \to \infty } \frac{a_{n}}{b_{n}}=\frac{A}{B}$, given $b\neq 0$.

