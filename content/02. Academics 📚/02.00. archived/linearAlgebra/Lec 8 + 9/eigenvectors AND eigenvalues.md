---
mindmap-plugin: basic
time: 
tags: 
source:
---
# eigenvectors AND eigenvalues
### description
- eigenvectors: vectors that are stretched or squashed during the transformation
- eigenvalue: the values of stretching or squashing during the transformation, can be negative or not exist
xz z
### solving
- finding eigenvec and eigenval of matrix A comes down to solving for $\lambda$ (scaling value - eigenvalues) and v (scaling vectors - eigenvectors), in $A\vec{v} = \lambda \vec{v}$ 
- to solve the eigenvalue $\lambda$, solve: $(A-\lambda I)\vec{v}=0$, 
- knowing that we dont want the eigenvectors v = 0, the matrix to solve is $(A-\lambda I)=0$, which looks like [this](https://i.imgur.com/405iy8e.png)
- fundamental behind (each bullet points are following inferences): 
	- equation $(A-\lambda I)\vec{v}=0$ -> the product of matrix with nonzero vector v = 0 
	- If the linear transformation (A - λI) squishes the space into a lower dimension -> the transformation must have a [[null space#description|nontrivial null space]]
		- The [[null space#description|null space]] of the transformation $(A - λI)$ is the set of all vectors v that satisfy the equation $(A - λI)v = 0$
		- The equation $(A - λI)v = 0$ implies that the linear transformation $(A - λI)$ maps every vector v to the zero vector => the transformation is not injective => det = 0 (see [[inference in LA|injection and determinant relation]])
	- it goes down to finding $det(A - λI) = 0$ 
		- eigenvalues: $\lambda$  
		- eigenvectors: replace $\lambda$ with the result found -> find v1, v2 vectors
		- $V = [v1\;v2]$  
		- S: ![](https://i.imgur.com/wKgf2xH.png)
<!--ID: 1708098042644-->

