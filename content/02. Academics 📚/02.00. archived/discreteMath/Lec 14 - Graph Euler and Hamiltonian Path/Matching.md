---
tags:
  - Math/discrete/graph/bipartite
---
# Matching
### Description:
- $M$, a subset $\in E$ such that no vertex in 𝑉 is on more than one edge in 𝑀
	- i.e. one $V$ has maximum one edge
### Perfect matching:
- Every vertex in $V$ is on an edge in $M$
<!--ID: 1708098041493-->

### Maximum matching:
- Largest possible of $|M|$, meaning the maximum number of connections between V1 and V2 as possible
<!--ID: 1708098041499-->

### Complete matching:
- $M$ such that every nodes in $V_1$ is matched (assumed $|V_1|\le |V_2|$)
- A complete match is a maximum match (as we have found the max matches for set V1), reverse is not true
<!--ID: 1708098041502-->

### Hall's marriage theorem:
- The bipartite graph 𝐺 = (𝑉, 𝐸) with bipartition $(V_1, V_2)$ has a complete matching from $V_1$ to $V_2$ if and only if $|N(A)|\ge |A|$ (number of neighbor vertices of A is $\ge$ than A) for all subsets of $A$ of $V_1$. #Math/discrete/graph/theorem 
	- Any subset of $V_1$ must have more matchable nodes then the number of nodes in $V_1$
	- note: $|N(A)|$ is neighbor of A
- Proof: lecture 14, slide 16
---
<!--ID: 1708098041505-->
