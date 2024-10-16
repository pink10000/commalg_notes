 A **local ring** is a ring with one *maximal ideal*. The technique of *localization* reduces problems to local rings. Many properties are preserved when rings become localized.

$$S = A - p \text{ is mulitplicatively closed} \iff p\text{ is prime}$$
So, $S^{-1}A = A_{p}$.
- elements $s / a$ form the only maximal ideal $M$ in $A_p$.

# Localization Properties
Let $A$ be `_______`. Then each local ring $A_p$ is `_______`.
1. [[Noetherian Ring]] 
2. [[Artinian Ring]]
3. [[Flat Module]]
4. [[Faithful Ring]]
5. [[Algebra]]
6. Integral Domain

The converse is not necessarily true.

# Module Properties
### Atiyah Proposition 3.8
Let $M$ be an $A-$module. Then the following are equivalent:
1)  $M = 0$
2) $M_{p} = 0$ for all prime ideals $p$ of $A$.
3)  $M_{m}= 0$ for all maximal ideals $m$ of $A$.

Proof. 
Clearly $1) \implies 2) \implies 3)$. Suppose $(3)$ holds and $M \neq 0$. Let $0 \neq x \in M$ and let $a \in \text{Ann}(x)$ for ideal $a \neq (1)$, and thus $a \subset m$ for $m$ the maximal ideal. We consider some $x / 1 \in M_m$. As $M_{m} = 0$ we have $x / 1 = 0$, and thus $x$ is killed by some element in $A - m$ but is impossible as $\text{Ann}(x) \subseteq m$. 

### Atiyah Proposition 3.9
Let $\phi : M \to N$ be an $A-$module [[Morphisms#Homomorphism|homomorphism]]. Then the following are equivalent:
1) $\phi$ is **injective**
2) $\phi_{p}: M_{p}\to N_{p}$ is **injective** for each prime ideal $p$. 
3) $\phi_{m} : M_{m}\to N_{m}$ is **injective** for each maximal ideal $m$.
Similarly, **injective** can be replaced with **surjective**. 