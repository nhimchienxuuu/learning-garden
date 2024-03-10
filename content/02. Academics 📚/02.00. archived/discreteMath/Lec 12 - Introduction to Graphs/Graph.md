---
tags:
  - Math/discrete/graph
aliases:
  - Graph theory
---
# Graph
### Description:
- From [[Seven Bridges of Königsberg]]
- a graph $G=(V,E)$ consists of $V$, a non-empty set of [[Vertex|vertices]] and $E$, a set of [[Edge|edges]]
### Finite vs infinite graph:
- A graph is called finite if both $|𝑉|$ and $|𝐸|$ are finite; otherwise, it is infinite.
<!--ID: 1708098041538-->

### Multigraph:
- Graphs that may have multiple edges connecting the same vertices
<!--ID: 1708098041542-->

### Pseudographs
- include loops, and possibly multiple edges
<!--ID: 1708098041546-->


### illustration of simple, multi, pseudo graphs
- [pic](https://image1.slideserve.com/2065357/types-of-graphs-l.jpg)
<!--ID: 1708098041550-->

### [[Undirected graph]]
### [[Directed graph]]

### Types:
| Туре | Edges | Multiple Edges Allowed? | Loops Allowed? | 
| ---- | ---- | ---- | ---- |
| **Simple graph** | Undirected | No | No |  
| Multigraph | Undirected | Yes | No |
| Pseudograph | Undirected | Yes | Yes |
| Simple directed graph | Directed | No | No |
| Directed multigraph | Directed | Yes | No | 
| Mixed graph | Directed and undirected | Yes | Yes | 
- Simple graph:
	- [[Complete Graph]]
	- Cycle:
		- for $n\ge 3$, the edges forms a cycle
		- There are $n$ edges in a cycle graph with $n\ge 3$ vertices
<!--ID: 1708098041555-->

### [[Graph representation]]
### [[Graph isomorphism]]
### [[Path]]
### Graph connectivity:
- An [[Undirected graph]] is connected if there exists a path between any two nodes $u,v\in V$ #Math/discrete/definition 
	- note that a graph containing a single node $v$ is considered connected via the length 0 path $(𝑣))$
	- An undirected graph that is not connected is called disconnected
- There is a simple path between every pair of distinct vertices of a connected undirected graph #Math/discrete/graph/theorem  
- A [[Directed graph]] is a **strongly connected** if there exists a path form any node $u$ to any node $v$ (so is from the node $v$ to node $u$) #Math/discrete/definition 
- A [[Directed graph]] is a **weakly connected** if there is a path between every 2 vertices in the underlying [[Undirected graph]] #Math/discrete/definition 
- A simple cycle of a particular length is a useful invariant that can be used to show that two graphs are **not isomorphic**.
<!--ID: 1708098041559-->

### Counting paths between vertices:
- Let 𝐺 be a graph with adjacency matrix 𝑨 with respect to the ordering $v_1, v_2,..,v_n$ of the vertices of  the graph (with directed or undirected edges, with multiple edges and loops allowed). 
- The number of different paths of length $r$ from $v_1$ to $v_j$ , where $r$ is a positive integer, equals the $(i,j)$th entry of $A^r$ #Math/discrete/graph/theorem 
	- the matrix power to r, then we have the number of possible ways of going from one node to the other
<!--ID: 1708098041563-->

### Subgraph:
- Given a graph $G=(V,E)$, a subgraph of $G$ is simply a graph $G'=(V',E')$ with $V'\subseteq V$ and $E'\subseteq (V'\times V')\cap E$.
	- We denote by $G'\subseteq G$
- A connected component of graph 𝐺 = (𝑉, 𝐸) is a maximal connected subgraph; that is, it is a subgraph 𝐻 ⊆ 𝐺 that is connected, and any larger subgraph 𝐻’  (satisfying 𝐻’ ≠ 𝐻, 𝐻 ⊆ 𝐻’ ⊆ 𝐺) must be disconnected.  
- We may similarly define a strongly connected component of a directed graph as a maximal strongly connected subgraph???
<!--ID: 1708098041567-->

### [[Bipartite Graph]]
### [[Planar Graph]]
### [[Graph Coloring]]
### [[Graph for Machine Learning]] 