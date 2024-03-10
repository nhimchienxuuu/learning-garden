---
mindmap-plugin: basic
time: 
tags: 
source:
---
# Low rank matrix approximations

### low rank matrix approximation
- special case of low rank approximation, where we use [[SVD]] to find optimal solution
- basically: 
	- rank-constrained approximation problem: $min_{A_k\in\mathbb{R}^{m,n}}||A-A_{k}||_{F}^{2}$ , such that $rank(A_k) = k$, given $1\leq k\leq r$
		- k is the parameter chosen based on how much info wanted to retain
		- k is small -> info is less accurate, efficient computation and storage
		- k is large -> info is accurate, more computation and storage
	- keeping only the first k largest singular values & the corresponding columns of U and V. This gives a new set of matrices $U_k, Σ_k,\;and\;V_k^T$
	- then, multiple these matrices to get the rank-k approximation of A
- help to minimize the Frobenius norm of the difference btw A and B (refer to Frobenius norm in [[Matrix properties via SVD#matrix norm|relation of F-norm with singular values]])
	- the ratio of the F-norm of B to F-norm of A is how much the info in A is captured by 
<!--ID: 1708098042542-->

