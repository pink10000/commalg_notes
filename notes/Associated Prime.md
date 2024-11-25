# Associated Primes
Let $R$ be a ring and a let $M$ be an $R-$module. 

A **prime idea**l $P$ of ring $R$ is **associated** to $M$ if $P$ is the **annihilator** of an element of $M$. The set of all primes associated to $M$ is written 
$$\text{Ass}_{R}M \;\;\text{or}\;\; \text{Ass}M$$
For $m \in M$,

$$P = \text{Ass}M = \text{Ann}(m) = \{r \;|\; rm = 0, r \in R\}$$
There is one exception:

If $I$ is an ideal of $R$, the the associated primes of the module $M = R/I$ are called **associated primes of $I$**. 

$P$ is not defined with some element $m \in M$ because
- many elements in $M$ can have the same associated prime
- $\text{Ass}(M)$ says more about the structure of $M$ as opposed to its elements. 

### Example
Let $R = \mathbb{Z}$, and $I = (6)$. Then $M = \mathbb{Z}/6\mathbb{Z}$ is the quotient module. The **associated primes** of $M$ are the prime ideal that are related to $(6)$.
$$\text{Ass}(\mathbb{Z} / 6\mathbb{Z}) = \{(2), (3)\}$$
## Theorem 3.1
Let $R$ be a [[Noetherian Ring]] and let $M$ be a finitely generated nonzero $R-$module.
1. $\text{Ass}M$ is a finite, nonempty set of primes, each containing $\text{Ann}(M)$. The set $\text{Ass}M$ includes all the prime ideals minimal among prime ideals that contain $\text{Ann}(M)$. 
	1. **Containment**: $P \in \text{Ass}_{R}(M) \implies \text{Ann}(M) \subseteq P$. Think about what $P$ does to one element in $M$.
	2. **Minimal**: The primes are called **primes minimal over $I$**.
	3. The primes not minimal are called **embedded primes of $M$**. 
	4. **Isolated Components**?
	5. **Embedded Components**?
2. The union of the associated primes of $M$ consists of $(0)$ and the set of zero divisors on $M$.
	1. Obvious by the annihilator.
3. The formation of the set $\text{Ass}M$ commutes with localization at an arbitrary manipulatively closed set $U$, in the sense that $$\text{Ass}_{R[u^{-1}]} = M[U^{-1}] = \{PR[U^{-1}] \;|\; P\in \text{Ass}M \wedge P \cap U = \emptyset\}$$
	1. We take the associated primes of $M$ and localize them, provided the prime ideals do not intersect $U$.
	2. Localization preserves associated prime structure.

## Corollary 3.2
Let $R$ be a Noetherian ring and let $M$ be a finitely generated nonzero $R-$module. Every ideal consisting entirely of zerodivisors on $M$ actually annihilates some element of $M$. 

#### Proof:
By [[Associated Prime#Theorem 3.1|Theorem 3.1]], an ideal $Z$ consisting of zerodivisors on $M$ is contained in the union of associated primes of $M$. By [[Prime Avoidance#Prime Avoidance Lemma|Prime Avoidance Lemma]], ideal $Z$ is contained in one of them.
