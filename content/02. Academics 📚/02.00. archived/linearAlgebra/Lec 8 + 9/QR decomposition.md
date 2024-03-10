---
mindmap-plugin: basic
time: 2024-01-15T01:58:00
tags: 
source:
---
# QR decomposition
### description
- to decompose (phân tích) matrix A into 2 constituent matrices (2 ma trận thành phần) Q and R, $A = Q.R$
- basically, nothing else than the gram-schmidt orthogonalization process
	- A: square + invertible matrix
	- Q: orthogonal matrix, with $Q^T = Q^{-1}$ => columns of Q form orthonormal basis
	- R: upper triangular matrix (all entries below the main diagonal are zero)
	- see [here](https://i.imgur.com/nuaThkj.png)
- find the orthonormal basis using [[gram-schmidt process]] -> find Q and R
	- $Q = [e_1 \cdots e_n]$
	- R as below
		- ![](https://i.imgur.com/XDi3cM0.png)

