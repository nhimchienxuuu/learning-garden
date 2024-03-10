---
tags:
  - Math/discrete/graph
---
# Title
### Description:
1. [Adjacency matrix](https://i.ytimg.com/vi/9C2cpQZVRBA/maxresdefault.jpg): 
	- A $n\times n$ matrix which has 1 at $[u][v]$ if $u$ points to $v$, otherwise 0
	- If the graph is undirected, then $a_{ij} = a_{ji}$ and the matrix 𝐴 is symmetric about the diagonal. 
		- Can be waste of memory
2. [Adjacency list](https://i.imgur.com/t6k3xq9.png):
	- 1 list for each vertex and it is 1 (or the weight) if it has edge to $u$
	- $E_v=\{u|(v,u)\in E\}$
3. [Edge list](https://i.imgur.com/7lAPPbA.png):
	- A list of all the edges, denoted by starting vertex and ending vertex
	- eg. ['A'. 'C']
### small quiz
- **True or False?**: For sparse graph (not so many edges), adjacent list and edge list are more memory efficient than adjacency matrix. => **True**
- adj matrix has to store a lot of unnecessary zeros of unconnected vertices
<!--ID: 1708098041531-->

