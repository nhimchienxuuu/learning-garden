---
mindmap-plugin: basic
time: 
tags: 
source:
---
# low rank models and projections
### description
- application of [[low rank approximation]] to represent data in lower-dimensional space

### projecting data points:
- Given a data matrix X with m columns (each column is a data point), each column xj is projected to a k-dimensional vector hj.
- This projection is done by multiplying xj with the transpose of the product of the k largest singular values and the k right singular vectors of X.
	- Project each data point xj to a k-dimensional vector hj: $h_{j}=V_{k}^{T}x_{j}$ 
<!--ID: 1708098042553-->


- with matrix X, use SVD to find rank-k approximation X' = UH
	- U: matrix of k orthogonal vectors
	- H: matrix of k coefficients
- each data point (column vector)
- each feature (row vector)