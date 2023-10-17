Series are the sum of [[Sequences]], where we take a sequence $(a_{n})_{n=1}^{\infty}$ and add up all of its terms.

# Convergence

> [!math|{"type":"definition","number":"auto","setAsNoteMathLink":false,"title":"Series","label":"series","_index":0}] Definition 1 (Series).
> A series $(a_{n})_{n=1}^{\infty}$ converges if the sequence of partial sums $S_{1}=a_{1}, S_{2}=a_{1}+a_{2}, S_{3}=a_{1}+a_{2}+a_{3}\dots$ converges. We then set $\sum_{k=1}^{\infty}a_{k}=\lim_{ n \to \infty }S_{n}$.

## Examples

Show that 

$$
\sum_{k=0}^{\infty}x^{k}=\frac{1}{1-x}, \, |x|<1
$$

`\begin{proof}`

Let 

$$
S_{n} = \sum_{k=0}^{n}x^{k} = x^{0} + x^{1} + \dots + x^{n}
$$

Then,

$$
xS_{n} = x\sum_{k=0}^{n}x^{k} = x^{1} + x^{2} + \dots + x^{n+1}.
$$

Subtracting the second equation from the first, we get

$$
\begin{gather}
S_{n}-S_{n}x = 1 - x^{n+1} \\
S_{n}(1-x) = 1-x^{n+1} \\
S_{n} = \frac{1-x^{n+1}}{1-x}.
\end{gather}
$$

Now, by the definition of convergence, we just need to make sure that $\lim_{ n \to \infty }S_{n}$ converges. Plugging in, we get

$$
\lim_{ n \to \infty } \frac{1-x^{n+1}}{1-x} = \frac{1}{1-x}.
$$

Therefore, 

$$
xS_{n} = x\sum_{k=0}^{n}x^{k} = x^{1} + x^{2} + \dots + x^{n+1}
$$

converges.
`\end{proof}`
## Sum of Two Converging Series

> [!math|{"type":"lemma","number":"auto","setAsNoteMathLink":false,"title":"Sum of 2 Converging Series","label":"sum-of--converging-series","_index":1}] Lemma 2 (Sum of 2 Converging Series).
> If $\sum a_{k}$ and $\sum b_{k}$ converge, then $\sum(\alpha a_{k}+\beta b_{k})$ converges for $\alpha,\beta \in \mathbb{R}$.

## Divergence of Harmonic Series

> [!math|{"type":"lemma","number":"auto","setAsNoteMathLink":false,"title":"Harmonic Series","label":"harmonic-series","_index":2}] Lemma 3 (Harmonic Series).
> $\sum_{k=1}^{\infty} \frac{1}{k}$ diverges. 

`\begin{proof}`

Observe that 

$$
\begin{align}
\sum_{k=n+1}^{2n} \frac{1}{k} &= \frac{1}{n+1} + \frac{1}{n+2} + \dots + \frac{1}{2n} \\
&> \frac{1}{2n} + \frac{1}{2n} + \dots + \frac{1}{2n} \\
&= \frac{n}{2n} = \frac{1}{2}
.\end{align}
$$

Therefore, 

$$
\begin{align}
\sum_{k=1}^{2^{S}} \frac{1}{k} &= \sum_{k=1}^{2} \frac{1}{k} + \sum_{k=3}^{4} \frac{1}{k} + \sum_{k=5}^{8} \frac{1}{k} + \dots + \sum_{k=2^{S-1}+1}^{2^{S}} \frac{1}{k} \\
&> \frac{S}{2}
\end{align}
$$

Thus, the set of partial sums diverges.
`\end{proof}`

## Telescoping Series

Similarly, $\sum_{k=1}^{\infty} \frac{1}{k+1}$ diverges. However, their difference $\sum_{k=1}^{\infty} \frac{1}{k} - \frac{1}{k+1}$ converges. This is because of telescoping series.

$$
\begin{align}
\sum_{k=1}^{\infty} \frac{1}{k} -\frac{1}{k+1} &= \frac{1}{1} - \frac{1}{2} + \frac{1}{2} - \frac{1}{3} + \frac{1}{3} - \frac{1}{4} \dots - \frac{1}{\infty} \\
&= 1
\end{align}
$$

## Necessary Limit Condition

> [!math|{"type":"lemma","number":"auto","setAsNoteMathLink":false,"title":"Limit of Converging Series Term","label":"limit-of-converging-series-term","_index":3}] Lemma 4 (Limit of Converging Series Term).
> If $\sum_{k=1}^{\infty} a_{n}$ converges, then $\lim_{ n \to \infty }a_{n}=0$.

`\begin{proof}`

$$
S_{n} = \lim_{ n \to \infty } \sum_{k=1}^{n}a_{k} = L \implies S_{n-1} = L \implies S_{n}- S_{n-1} = L - L = 0 = a_{n}
$$
`\end{proof}`

## Comparison Test

If $\sum_{}^{}b_{n}$ converges and $a_{n} \leq c b_{n}$ for $n\geq 1, c > 0$, then $\sum_{}^{}a_{n}$ converges.

`\begin{proof}`This is obvious when comparing partial sums (both are bounded). `\end{proof}`

## Limit Comparison Test

If $a_{n}, b_{n} > 0$ and $\lim_{ n \to \infty } \frac{a_{n}}{b_{n}} = 1$, then $\sum_{}^{}a_{n}$ converges iff $\sum_{}^{}b_{n}$ converges.

`\begin{proof}`$\lim_{ n \to \infty } \frac{a_{n}}{b_{n}} = 1 \implies \exists N \in \mathbb{N}$ such that $\frac{1}{2} < \frac{a_{n}}{b_{n}} < \frac{3}{2}$ for $n \geq N \implies b_{n} < 2a_{n}, a_{n} < \frac{3}{2} b_{n}$ for $n \geq N$. Then, we can apply Comparison Test.
`\end{proof}`

## Root Test

If $a_{k}\geq 0$ for $k\geq 1$ in $\sum_{k=1}^{\infty}a_{k}$ and $\lim_{ n \to \infty }a_{k}^{\frac{1}{k}} = R$, then 

1. If $R < 1$, the series converges ($a_{n}=\frac{n}{3^{n}}$)
2. If $R>1$, the series diverges ($a_{n}=n^{2}2^{n}$)
3. If $R=1$, inconclusive ($a_{n}=\frac{1}{n\log n}$)

`\begin{proof}` If $R<1$, choose $x$ such that $R<x<1$. Then, $\exists N \mid a_{n}^{\frac{1}{n}} < x$ for $n\geq N$. Then, $a_{n} < x^{n}$ for $n\geq N$ and $x < 1 \implies x^{n} \to 0$. 

If $R > 1$, then $\lim_{ n \to \infty }a_{n} \neq 0$.
`\end{proof}`

## Ratio Test

