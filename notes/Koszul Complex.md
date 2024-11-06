



# Simple Koszul Complexes
$$K(x):0 \to R \to_{x} R$$
1.  $K(x)$ only contains one element, $x$, so it is length $1$. The map is simply $y \mapsto xy$ .
2. The [[Complex#Homology|Homology]] is $\text{ker}(x) / \text{im}(0) = 0 / R = 0$.


Given a second element $y \in R$, **multiplication** by $y$ is a map:
```tikz
\usepackage{tikz-cd}
\begin{document}
    \begin{tikzcd} {K(x):0} & R & R \\ {K(x):0} & R & R \arrow[from=1-1, to=1-2] \arrow["x", from=1-2, to=1-3] \arrow["y"', from=1-2, to=2-2] \arrow["y", from=1-3, to=2-3] \arrow[from=2-1, to=2-2] \arrow["x", from=2-2, to=2-3] \end{tikzcd}
\end{document}
```
We can define a larger complex $K(x,y)$ because $R$ is a [[Free Module]]:
```tikz
\usepackage{tikz-cd}
\begin{document}
\begin{tikzcd} 
	0 & R & R & 0 & .\\ 
	 . & 0 & R & R & 0 
	\arrow[from=1-1, to=1-2] 
	\arrow["x", from=1-2, to=1-3] 
	\arrow["y"', from=1-2, to=2-3] 
	\arrow[from=1-3, to=1-4] 
	\arrow["y", from=1-3, to=2-4] 
	\arrow[from=2-2, to=2-3] 
	\arrow["-x", from=2-3, to=2-4] 
	\arrow[from=2-4, to=2-5] 
\end{tikzcd}
\end{document}
```
We note that the bottom is $-x$ to ensure that it becomes an [[Exact Sequence]]. More simply, we are taking the direct sum of the two complexes:
```tikz
\usepackage{tikz-cd}
\begin{document}
\begin{tikzcd}[cramped] 0 & {R \oplus 0} & {R \oplus R} & {0 \oplus R} & 0 \arrow[from=1-1, to=1-2] \arrow[from=1-2, to=1-3] \arrow[from=1-3, to=1-4] \arrow[from=1-4, to=1-5] \end{tikzcd}
\end{document}
```
Or even simpler,
```tikz
\usepackage{tikz-cd}
\begin{document}
\begin{tikzcd} 0 & R & {R^2} & R \arrow[from=1-1, to=1-2] \arrow["{y \choose -x}", from=1-2, to=1-3] \arrow["{(x,y)}", from=1-3, to=1-4] \end{tikzcd}
\end{document}
```
Where the vectors come from the fact that we are mapping $R \to R^2$ or in a very juvenile way, "increase dimension", then "reduce dimension".   