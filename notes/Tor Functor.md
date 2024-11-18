Let $R$ be a ring. The $\text{Tor}$ [[Functors|Functor]] is defined as:
$$ \begin{aligned}
\text{Tor}_{i}^{R}(-, N): R\textbf{-Mod} &\longrightarrow R\textbf{-Mod} \\
M &\longmapsto \text{Tor}_{i}^{R}(M, N)
\end{aligned} $$
where 
$$\text{Tor}_{i}^{R}(M, N) = H_{i}(K \otimes N)$$
the [[Homology|homology]] of [[Complex|complex]] $K$ tensored by $R-$module $N$. 
- The $\text{Tor}$ functor "measures" the exactness of a complex. 


## Short [[Exact Sequence]] 
Given SES
$$0 \to A \to B \to C \to 0$$
We have the following:
$$ \begin{aligned}
\cdots &\to 
\text{Tor}_{2}^{R}(A, N) \to \text{Tor}_{2}^{R}(B, N) \to \text{Tor}_{2}^{R}(C, N) \\ 
&\to \text{Tor}_{1}^{R}(A, N) \to \text{Tor}_{1}^{R}(B, N) \to \text{Tor}_{1}^{R}(C, N) \\
&\to \text{Tor}_{0}^{R}(A, N) \to \text{Tor}_{0}^{R}(B, N) \to \text{Tor}_{0}^{R}(C, N) \to 0
\end{aligned} $$
where for some $k$, $\text{Tor}_{k}^{R}(-,N) = 0$ which is our measure of exactness. 

## Properties
- $\text{Tor}_{0}^{R}(A, B) = A\otimes_{R}B$ when $i = 0$


### Example
Let $K$ be an SES:
$$0 \to \mathbb{Z}_{2} \to \mathbb{Z}_{6} \to \mathbb{Z}_{3} \to 0$$
Clearly, $\text{Tor}_{0}^{\mathbb{Z}}(-,\mathbb{Z}_{9})$ is 
$$
\cdots \to \mathbb{Z}_{2} \otimes \mathbb{Z}_{9} \to \mathbb{Z}_{6}\otimes \mathbb{Z}_{9} \to \mathbb{Z}_{3}\otimes \mathbb{Z}_{9} \to 0
$$
Now, to find $\text{Tor}_{1}^{\mathbb{Z}}(-, \mathbb{Z}_{9})$, we need to take the [[Projective Resolution|projective resolution]] of each module and find the [[Homology|homology]].