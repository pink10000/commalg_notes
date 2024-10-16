An **algebraic set** $X$ in [[Affine Space]] of dimension $r$ over $k$ is a set defined by a collection of polynomials, in which all points $x \in X$ are the roots of all the polynomials in the collection.
$$X = \{(x,y) \in \mathbb{A}^2  \;|\; x^2 + y^2 - 1 = 0 \}$$
This algebraic set defines the solutions to a circle in $\mathbb{A}^2$. 

## Irreducible
An algebraic set $X$ in affine $r-$space over $k$ is called **irreducible** if it cannot be expressed as the union of two *properly smaller* algebraic sets. 
$$X = X_{1} \cup X_{2}$$
Note that *properly smaller* means that $X_{i}\subsetneq X$. 

### Example
An example of reducible algebraic set is
$$X \subseteq \mathbb{A}^{2}(\mathbb{C})$$
defined by the polynomial
$$f(x,y) = (x-1)(x+1) = 0$$
such that 
$$X = \{(1,y) \;|\; y \in \mathbb{C}\} \cup 
\{(-1,y)\;|\; y \in \mathbb{C}\}
$$
which shows it is reducible.

### Theorem
$$\text{If $I \subset k[x_{1}, x_{2}, \cdots x_{r}]$ is the ideal of $X$, then $X$ is irreducible iff $I$ is prime. }$$

- If $X$ is irreducible, and $fg \in I$, then $Z(I, f) \cup Z(I,g) = X$ in which both are the algebraic sets defined over $f$ and $g$ respectively. $f,g$ must vanish (evaluate to $0$) and be in $I$. As $X$ is irreducible, either $Z(I,f)$ or $Z(I,g)$ vanishes on all points in $X$. Indeed, either $f$ or $g$ vanishes on points of $X$. Thus, as $fg \in I$ and only either $f,g \in I$, $I$ is prime.

- Conversely, suppose $X = X_{1} \cup X_2$ such that $X$ is not irreducible. If each $X_i$ is an algebraic set smaller than $X$, then there is a function $f_i$ vanishing on $X_i$ but not $X$ by definition. Since $f_1f_2$ vanishes on $X$, and $I$ is prime, either $f_1$ or $f_2$ vanish on all of $X$, violating the assumption that $f_{1},f_{2}$ do not vanish on all of $X$, and so $X$ must be irreducible.

