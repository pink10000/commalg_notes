Let $C,D$ be two categories. A **covariant functor** 
$$\mathscr{F} : C \to D$$
is an assignment of an object $\mathscr{F}(A)\in \text{Obj}(D)$ for every $A \in \text{Obj}(C)$ and of a function
$$\text{Hom}_{C}(A,B) \to \text{Hom}_{D}(\mathscr{F}(A), \mathscr{B}(B))$$
for every pair of objects $A,B$ in $C$. This function must preserve *identities* and *compositions*. That is,
$$\mathscr{F}(1_{A}) = 1_{\mathscr{F}(A)}$$
for all $A \in \text{Obj}(C)$, and
$$\mathscr{F}(\beta \circ \alpha) = \mathscr{F}(\beta) \circ \mathscr{F}(\alpha)$$
$\forall A, B, C \in \text{Obj}(\textbf{C}), \forall \alpha \in \text{Hom}_{\textbf{C}}(A,B), \forall \beta \in \text{Hom}_{\textbf{C}}(B,C)$.

A **contravariant** functor $C \to D$ is a covariant functor $C^{op} \to D$ from the opposite category. 

# Opposite Categories
$C^{op}$ is obtained from "reversing the arrows" of a category.

