> [!math|{"type":"definition","number":"auto","setAsNoteMathLink":false,"title":"exp","label":"exp","_index":0}] Definition 1 (exp).
> The inverse function of $\log$ from $\mathbb{R} \to \mathbb{R}^{+}$ is $\exp(x)$.

# Properties

> [!math|{"type":"proposition","number":"auto","setAsNoteMathLink":false,"_index":1}] Proposition 2.
> $\exp(0)=1$

`\begin{proof}`$\exp(\log(y))=y, \log(1)=0$. `\end{proof}`

> [!math|{"type":"proposition","number":"auto","setAsNoteMathLink":false,"_index":2}] Proposition 3.
> $\frac{d}{dx}\exp=\exp$

`\begin{proof}`Since $\frac{d}{dx}\log x=\frac{1}{x}\neq 0$, using [[Differentiation#Derivatives of Inverses|the formula for the derivative of an inverse]], 

$$
\frac{d}{dx}\exp(x)=\frac{1}{\frac{d}{dx}\log(\exp(x))}=\frac{1}{\frac{1}{\exp(x)}}=\exp(x)
$$
`\end{proof}`

> [!math|{"type":"proposition","number":"auto","setAsNoteMathLink":false,"_index":3}] Proposition 4.
> For $x,y \in \mathbb{R}$, $\exp(x+y)=\exp(x)\exp(y)$

`\begin{proof}` For $x,y \in \mathbb{R}$, exists unique $u,v \in \mathbb{R}^{+}$ s.t. $x=\log u,y=\log v$.

$$
\begin{align}
\exp(x+y)&= \exp(\log u+\log v) \\
&= \exp(\log uv) \\
&= 
\end{align}
$$
`\end{proof}`

> [!math|{"type":"proposition","number":"auto","setAsNoteMathLink":false,"_index":4}] Proposition 5.
> $\exp$ is strictly increasing.

> [!math|{"type":"proposition","number":"auto","setAsNoteMathLink":false,"_index":5}] Proposition 6.
> $\lim_{ x \to \infty }\exp(x)=\infty$, $\lim_{ x \to -\infty }(x)=0$

> [!math|{"type":"proposition","number":"auto","setAsNoteMathLink":false,"_index":6}] Proposition 7.
> $\int \exp(x) \, dx=\exp(x)+C$

> [!math|{"type":"proposition","number":"auto","setAsNoteMathLink":false,"_index":7}] Proposition 8.
> $\lim_{ x \to \infty } \frac{p(x)}{\exp(x)}=0$ and $\lim_{ x \to \infty }p(x)\exp(x)$ for polynomials $p$.

> [!math|{"type":"proposition","number":"auto","setAsNoteMathLink":false,"_index":8}] Proposition 9.
> $\int_{-\infty}^{b} \exp(x) \, dx=\exp(b)$