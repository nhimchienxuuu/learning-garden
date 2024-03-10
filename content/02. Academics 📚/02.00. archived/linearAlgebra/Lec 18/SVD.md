---
mindmap-plugin: basic
time: 2024-01-15T22:23:00
tags: []
source:
---
# SVD
### description
?
- similar to spectral factorization 
- any non-zero matrix $A \in R^{m,n}$, can be factored as $A=U{\tilde{S}}V^{T}$
	- $U$: orthogonal matrix, $\in R^{m,m}$. columns of U: left-singular vectors
	- $\tilde{S}$: diagonal, positive & decreasing in magnitude entries
	- $V$: orthogonal matrix, $\in R^{n,n}$. columns of V: right-singular vectorsf

### finding SVD of matrix C
?
0. want to find $C = USV^T$
1. Knowing that $C^TC = VS^TU^TUSV^T = VS^TSV^T$, find $C^TC$ -> find $V$ and $S$
	- find $C^TC$
	- find $det(C^TC - \lambda I)$ = 0 (finding [[eigenvectors AND eigenvalues]])
2. From $CV = U.S$ -> find $U = C.V.S^T$
<!--ID: 1708098042360-->


### compact form SVD
?
- any non-zero matrix $A \in R^{m,n}$ can be expressed as: $A = U_r.S.V_r^T$



### SVD from dyads view (lec 19)
- any matrix $A \in R^{m,n}$, rank $r$ > 0 can be expressed as sum of "orthogonal dyads"
- $A=\sum_{i=1}^{r}\sigma_{i}u_{i}v_{i}^{\top}$
	- $u_1, \cdots, u_r \in R^m$ , $v_1,\cdots,v_r \in R^n$ are mutually orthogonal collections of vectors
	- $\sigma_1 \geq \cdots \geq \sigma_r > 0$
	- now completing these collections with vectors $v_i \in R^m, i=1,\cdots,n$ and $u_i \in R^m, i = r+1,\cdots,m$, so that $U = u_1, \cdots, u_m$ and $V = [v_1,\cdots, v_n$ ] are both orthonormal matrices
<!--ID: 1708098042369-->


