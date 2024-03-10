---
mindmap-plugin: basic
create-time: 
tags:
---
# Introduction to Graphs
## Definition of Graphs
### Definition of Graph
- graph $G = (V, E)$
- V: non empty set of vertices (nodes)
- E: set of edges connecting its endpoints, with each edge has 1 or 2 vertices associated with it (called endpoints)
<!--ID: 1708098042113-->


### Finite vs Infinite graph:
- finite: both |V| and |E| are finite
- infinite: otherwise
<!--ID: 1708098042118-->


### Simple graph:
- Each edge connects two different (unordered) vertices: [[Pasted image 20231214224505.png|here]]
- No 2 edges connect same pair of vertices: [[Pasted image 20231214224519.png|here]]
- no edge connects a vertex to itself (loop): [[Pasted image 20231214224532.png|here]]
<!--ID: 1708098042122-->


### Multigraph
- graphs of multiple edges connecting the same vertices
<!--ID: 1708098042126-->


### Pseudographs
- include loops, possibly multiple edges
<!--ID: 1708099388768-->


### Undirected graph
- all edges are undirected
- ie. unordered pairs (or set) {u, v}
<!--ID: 1708098042131-->


## Directed graphs (digraph)
- Traits
	- (V,E)
	- non empty set of vertices V
	- set of directed edges (arcs)
	- each directed edge associate with ordered pair of vertices, i.e. (u,v), and start at u and end at v
- Different graphs types
	- Simple directed graph
		- no loop, no multiple directed edges
	- directed multigraphs
		- have multiple directed edges from a vertex to a second (possibly the same) vertex
	- multiplicity m
		- m directed edge from (u,v)
	- mixed graph
		- both undirected and directed edges
	- hypergraph
	- summary: [[Pasted image 20231214231351.png|here]]
<!--ID: 1708098042137-->


## Terminology
- Adjacent/ neighbor: a and b vertices are called adjacent if it is connected by an edge e
- Neighborhood: 
	- $N(x) = \{a,b,c,d\}$ in which vertex v is adjacent to a,b,c,d
	- $N({x,y}) = N(x) \cup N(y) = \{f\}$
- degree of a vertex:
	- undigraph:
		- number of edges adjacent to it, loop = +2 to the deg
		- $deg(v)$
		- *Handshaking theorem*: 
			- $2m = \sum_{v\in V} deg(v)$: total number of degrees is two times the edges
			- undigraph has EVEN number of vertices of ODD degree
				- prove by showing $2m = \sum_{v\in V_1} deg(v) + \sum_{v\in V_2} deg(v)$, each of the 3 terms are even ($V_1$: set of vertices of even degree, $V_2$: set of vertices of odd degree)
				- but all terms in $\sum_{v\in V_2} deg(v)$ are odd -> even number of such terms -> $|V_2|$ is even
	- digraph:
		- [[MATH2020 (Lec 12) - Introduction to Graphs#^0f3d92|here]]
	- pendant: vertex of deg = 1
	- isolate: vertex of deg = 0
<!--ID: 1708098042141-->


## Graph representations
- impact: affect storage size, efficiency of various graph algorithms
- Adjacency matrix
	- space complexity: $n^2$
	- illustration: [[Pasted image 20231214232925.png|here]]
- Adjacency list
	- illustration: [[Pasted image 20231214233251.png|here]]
- Edge list
	- illustration: [[Pasted image 20231214233341.png|here]]
	- set of vertices that have at least one edge entering or leaving, denoted in the right order
<!--ID: 1708098042145-->


## Directed graph
- definition & terms
	- a -> b, with (a,b) is an edge in graph G
		- vertex a is adjacent TO b
	- b -> c, with (b,c) is an edge in graph G
		- vertex c is adjacent FROM b
- degrees ^0f3d92
	- in-degree: $deg^{-}(a)$: a is the terminal (end) vertex
	- out-degree: $deg^{+}(b)$: b is the initial (start) vertex
	- $\Sigma_{v\in V}\,deg^{-}(v)\,=\,\Sigma_{v\in V}\,deg^{+}(v)\,=\,|E|$: sum all in and out degrees is equal to total no. of edges
		- prove: each connection will contribute 1 to in-deg and 1 to out-deg
<!--ID: 1708098042149-->


## Special simple graphs
- complete graph on n vertices or $K_n$: simple graph, exactly 1 edge btw each pair of distinct vertices
	- $\frac{n(n-1)}{2}$ edges in a complete graph with $n\geq 2$ vertices
- noncomplete graph: simple graph, at least 1 pair of distinct vertices not connected by an edge
<!--ID: 1708098042153-->
