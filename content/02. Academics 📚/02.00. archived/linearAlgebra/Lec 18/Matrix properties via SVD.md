---
mindmap-plugin: basic
time: 
tags: 
source:
---

# Matrix properties via SVD
### rank, nullspace, range
?
- rank $r$ of matrix A, is the maximum number of linear independent rows or columns of A (refer to [[range AND rank]])
- in SVD, rank $r$ is also the number of nonzero [[singular values]] / nonzero entries on the diagonal of S
- $dim\;N(A) = n-r$ (refer to [[fundamental theorem of linear algebra]])
- an orthonormal basis spanning N(A): $N(A) = R(V_{nr})$, $V_{nr} = [v_{r+1} \cdots v_n]$ 
- an orthonormal basis spanning the range of A: $R(A) = R(U_r), U_r = [u_1 \cdots u_r]$ 
<!--ID: 1708098042376-->


### matrix norm
?
- squared frobenius matrix norm = sum of the diagonal elements of the matrix $A^TA$ (trace) = sum of the singular values squared
	- $||A||_{F}^{2}=\mathrm{trace}\,A^{T}A=\sum_{i=1}^{n}\sigma_{i}^{2}$ 
		- $\sigma_{i}^{2}$: singular values of A 
- $I_2$ induced norm $||A||_2$ = largest singular value
	- $||A||_{2}=\operatorname*{max}_{x\neq0}{\frac{\|A x\|_{2}}{\|x\|_{2}}}\equiv\sigma_{1}$ 
<!--ID: 1708098042379-->
