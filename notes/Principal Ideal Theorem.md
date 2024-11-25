# Eisenbud
If $x \in R$ and $P$ is minimal among primes of $R$ containing $x$, then the height of $P \leq 1$.
- minimal by inclusion
- if $x$ is a unit, then no primes contain it
- If $Q \subset R$ is a prime ideal, then the $n$th [[Symbolic Power|symbolic power]] 
 $$Q^{(n)} = \{r \in R | sr \in Q^{n} \text{ for some } s \in R, s \not\in Q\}$$
  is the preimage in $R$ of the $n$th power of the localized ideal $Q_{Q}$ in $R_{Q}$. The elements outside $Q$ are non-zerodivisors mod $Q^{(n)}$ and on localization we get
$$(Q^{n})_{Q} = (Q_{Q})^{n}$$
#### Proof:
We shall show that if $Q$ is any prime ideal with $Q \subsetneq P,$ then $R_{Q}$ has dimension $0$, so height $Q = 0$. This shows that height of $P \leq 1$.

Replacing $R$ by $R_{P}$ we may assume that $P$ is maximal, and we have ideals as in:
```tikz
\usepackage{tikz-cd}
\begin{document}
\begin{tikzcd} & R \\ & P \\ {(x)} && Q \arrow[no head, from=1-2, to=2-2] \arrow["{Q^{(n)} + (x)}"{description}, no head, from=2-2, to=3-1] \arrow[no head, from=2-2, to=3-3] 
\end{tikzcd}
\end{document}
```
Since $P$ is minimal over $(x)$, the ring $R/(x)$ is [[Artinian Ring|Artinian]] by Theorem 2.14. Thus the descending chain
$$(x) + Q^{(n)}$$
stabilizes, say with 
$$Q^{(n)} \subset (x) + Q^{(n + 1)}$$
It follows that for any $f \in Q^{(n)}$ we may write $f = ax + g$ with $g \in Q^{(n+1)}$. This implies that $ax \in Q^{(n)}$. Since $P$ is minimal over $(x)$, we have 
$$x \not\in Q \implies a \in Q^{(n)}$$
From this we see that
$$Q^{(n)} = (x)Q^{(n)} + Q^{(n+1)}$$
Since $x \in P$, [[Nakayama's Lemma]], Corollary 4.8a, implies $Q^{(n)} = Q^{(n+1)}$. A second application of [[Nakayama's Lemma]], this time in $R_{Q}$, yields $(Q_{Q})^{n} = 0$, so $R_{Q}$ has dimension $0$ as claimed.
