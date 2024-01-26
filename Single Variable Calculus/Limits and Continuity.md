# Limits

Let $a \in \mathbb{R}$. Assume $f$ is [[Single Variable Calculus/Functions|function]] defined on some [[Single Variable Calculus/Functions#Intervals|neighborhood]] of $a$, except maybe $a$ itself.

Here are 3 definitions of a limit.

> [!definition] Epsilon Delta
> %% label: epsilon-delta %%
> $f$ has limit $A$ as $x \to a$ iff for every $\epsilon>0$, $\exists \delta>0 : |f(x)-A| < \epsilon$, $\forall x: |x-a| < \delta, x \neq a$. We write $\lim_{ x \to a }f(x)=A$.

Sometimes a function is defined piecewise on different sides of $x \in X$. Then, there is a left limit and right limit. 

> [!definition] Left Limit
> %% label: left-limit %%
> $\lim_{ x \to a^{+} }f(x)=A$ $\iff$ $\forall\epsilon>0$, $\exists \delta > 0 : 0 < x - a < \delta \implies |f(x)-A|<\epsilon$.

> [!definition] Right Limit
> %% label: right-limit %%
> $\lim_{ x \to a^{+} }f(x)=A$ $\iff$ $\forall\epsilon>0$, $\exists \delta > 0 : 0 < a-x < \delta \implies |f(x)-A|<\epsilon$.

Then,

> [!definition] Right and Left Limit
> %% label: right-and-left-limit %%
> $\exists\lim_{ x \to a } f(x) \iff \exists\lim_{ x \to a^{+} }f(x) \land \exists\lim_{ x \to a^{-} }f(x)$.

Notice that the following are equivalent:

1. $\lim_{ x \to a }f(x)=A$
2. For every sequence $(a_{n})_{n=1}^{\infty} \subset X$ where $f: X \to Y$, with $a_{n}\neq a$ for $n\geq 1$ and $a_{n} \to a$, $\lim_{ n \to \infty }f(a_{n})=A$.

`\begin{proof}`

$1 \implies 2$:
Given $\epsilon>0$, pick $\delta>0$ such that $|x - a| <\delta \implies |f(x)-A| < \epsilon$. Since $a_{n} \to a$, we know $\exists N \in \mathbb{N}:n \geq N \implies |a_{n}-a|<\delta \implies |f(a_{n})-A| < \epsilon$.

$2 \implies 1$:
We will prove the contrapositive. Pick $\epsilon>0:\not\exists\delta$ for the epsilon-delta condition. Then, if we let $a_{n}=x (\frac{1}{n})$, $a_{n} \to a$ but $f(x) \neq A$ by our assumption that $1$ is false. Thus, $2$ is false.
`\end{proof}`

$1 \iff 2$ is very powerful because can use sequences to prove properties of limits. For example,

> [!theorem]
> Let $A=\lim_{ x \to a }f(x)$ and $B=\lim_{ x \to a }g(x)$. Then,
> $$
> \begin{gather}
> \lim_{ x \to a } f(x) + g(x) = A + B \\
> \lim_{ x \to a } f(x) - g(x) = A - B \\
> \lim_{ x \to a } \frac{f(x)}{g(x)} = \frac{A}{B} \text{ if } b \neq 0
> \end{gather}
> $$

is true because we can proven the corresponding statements for sequences. Another example is 

## Squeeze Principle

> [!theorem] Squeeze Principle
> %% label: squeeze-principle %%
> If $f(x)\leq g(x)\leq h(x)$ in some neighborhood of $a$ and $\lim_{ x \to a }f(x)=\lim_{ x \to a }h(x)=A$, then $\lim_{ x \to a }g(x)=A$.

## Limits at Infinity

> [!definition] Limit at Infinity
> %% label: limit-at-infinity %%
> $\lim_{ x \to \infty }=A \iff$ $\forall\epsilon>0, \, \exists T>0: |f(x)-A|<\epsilon$ for all $x>T$. $\lim_{ x \to -\infty }f(x)$ is defined similarly.

## [[L'Hopital's Rule]]

Used for indeterminate forms.

# Continuity

> [!definition] Continuity
> %% label: continuity %%
> $f$ is continuous at point $a$ if $f$ is defined at $a$ and $\lim_{ x \to a }f(x)=f(a)$. $f$ is continuous if it is continuous at every point where it is defined.

- jump discontinuity: left and right limits exist but aren't equal
- removable discontinuity: limit exists but not equal to $f(a)$; can redefine to remove discontinuity

> [!proposition]
> $f$ is continuous at $a$ and $g$ is continuous at $b = f(a)$ $\implies$ $g\circ f: x \to g(f(x))$ is continuous at $a$.

^f84bec

`\begin{proof}` Continuity of $g$ at $f(a)$ implies $\forall\epsilon>0$ $\exists \eta>0:$ $|y-f(a)|<\eta \implies g(y)-g(f(a)) < \epsilon$. 

Continuity of $f$ at $a$ $\implies$ $\forall \eta>0$, $\exists\delta>0: |x-a|<\delta \implies |f(x)-f(a)| < \eta$. Thus, $|x<a| < \delta$ $\implies |f(x)-f(a)| < \eta \implies |g(f(x)) - g(f(a)) < \epsilon$, so $g\circ f$ is continuous at $a$. 
`\end{proof}`

[[#^f84bec]]  is useful for creating new continuous functions. Another useful proposition is 

> [!proposition]
> If $f$ is continuous at $a$ and $(x_{n})_{n=1}^{\infty}$ with $x_{n} \to a$ as $n \to \infty$, then $f(x_{n}) \to f(a)$ as $n \to \infty$.

^9f10f9

[[#^9f10f9]] is useful to prove discontinuity. For example, to show $\sin(\frac{1}{x})$ is discontinuous at $x=0$

`\begin{proof}` Consider the sequence $x_{n} = \frac{1}{\pi n}$ with $x_{n} \to 0$. Then $\sin(\frac{1}{x_{n}} = \sin \pi n = (-1)^{n} \not \to 0$ as $n \to \infty$.
`\end{proof}`
