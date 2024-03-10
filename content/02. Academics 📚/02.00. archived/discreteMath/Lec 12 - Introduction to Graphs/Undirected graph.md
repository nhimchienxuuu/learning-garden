---
tags:
  - Math/discrete/graph
---
# Undirected
### Description:
- All edges are undirected
### terminology
1. **adjacent (neighbors)**: if 2 endpoints a, b are connected with an edge e
	- a and b are adjacent
	- w is incident with b and c
2. **neighborhood**
	- $N(f) = \{b,a,e,c\}$
	- $N({a ,b}) = N(a) \cup N(b) = \{f\}$ 
3. **degree in undirected graph**
	- number of edges incident with it, with a loop counted twice to the degree of that vertex
	- $deg(v)$
	- *pendant*: vertex with degree 1
	- *isolate*: vertex with degree 0
<!--ID: 1708098041578-->

### Handshaking theorem:
- definition: find sum of degrees or total edges of a undirected graph
	- Let $𝐺 = (𝑉, 𝐸)$ be an undirected graph with 𝑚 edges. 
	- Then  $\displaystyle 2m = \Sigma_{v\in V}\text{deg}(𝑣)$ (sum of total degrees = 2 x edges)
- Also applies even if multiple edges and loops are present.
- Theorem:
	- An undirected graph has an even number of vertices of odd degree #Math/discrete/graph/theorem 
<!--ID: 1708098041583-->


