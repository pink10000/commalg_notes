A **Graded Ring** is a ring that has a decomposition into additive subgroups indexed by the integers. 

Formally,
$$R = \bigoplus_{n \in \mathbb{Z}} R_{n}$$
where $R_{n}$ is an additive subgroup (or module of $R$) such that
- multiplication respects the grading. $r \in R_{m} \wedge s \in R_{n}\implies r \cdot s \in R_{m + n}$
- the degree of the product of two elements in the sum of their degrees 


# Example 1: Polynomial Ring
$R = k[x_{1}, \cdots x_{n}]$ over a field $k$ is a graded ring by assigning a **degree** to each monomial. 
$$R = \bigoplus_{d \geq 0} R_{d}$$
where $R_{d}$ is the set of all **homogeneous polynomials** of degree $d$, or the the polynomials where the sum of exponents of all terms is exactly $d$. 

If $R = k[x,y]$ then 
$$R_{0} = k, \quad R_{1}= \{ax + by \;|\; a,b \in k\} \quad R_{2} = \{ax^{2}+ bxy + cy^{2}\;|\; a,b,c \in k\}$$

