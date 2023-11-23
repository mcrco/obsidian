> [!math|{"type":"definition","number":"auto","setAsNoteMathLink":false,"title":"Natural Logarithm","label":"natural-logarithm","_index":0}] Definition 1 (Natural Logarithm).
> For any $x>0$, we define its natural logarithm by
>
> $$
> \log x = \ln x = \int_{1}^{x} \frac{dt}{t}
> $$

# Properties

> [!math|{"type":"proposition","number":"auto","setAsNoteMathLink":false,"_index":1}] Proposition 2.
> $\log 1=0$

> [!math|{"type":"proposition","number":"auto","setAsNoteMathLink":false,"_index":2}] Proposition 3.
> $\log x$ is differentiable on $(0,\infty)$ with derivative $\frac{1}{x}$

`\begin{proof}`For any $x$, the function $\frac{1}{t}$ is continuous on $[1,x]$, so by the [[Fundamental Theorem of Calculus#The First Fundamental Theorem of Calculus|first fundamental theorem of calculus]], $\log x$ is differentiable with derivative $\frac{1}{x}$.`\end{proof}`

> [!math|{"type":"proposition","number":"auto","setAsNoteMathLink":false,"_index":3}] Proposition 4.
> For all $x,y>0$, $\log xy = \log x + \log y$.

`\begin{proof}``\end{proof}`

4. $\log x$ is strictly increasing on $(0,\infty)$
5. $\log x \to \infty$ as $x -< \infty$ and $\log x \to -\infty$ as $x \to \infty$
6. $\log x$ is integrable on any finite subinterval of $(0,\infty)$ and 

$$
\int \log x \, dx = x\log x - x + C 
$$

7. 

$$
\lim_{ x \to 0 } x\log x=0 \quad \text{and} \quad \lim_{ x \to 0 } \frac{\log x}{x} = 0
$$

8. Improper integral of $\log x$ over $(0,b]$ exists for any $b>0$ and 

$$
\int_{0}^{b} \log x \, dx =b\log b - b.
$$
