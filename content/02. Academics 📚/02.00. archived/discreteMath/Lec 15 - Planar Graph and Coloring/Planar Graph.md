---
tags:
  - Math/discrete/graph
mindmap-plugin: basic
time: 
source:
---
# Planar Graph
### Description:
- A graph that can be drawn in the plane **without any edges crossing**
	- where a crossing of edges is the intersection of the lines or arcs representing them at a point other than their common endpoint.
	- such drawing is called "Planar representation"
	- ![|300](https://i.imgur.com/C7ZMmgx.png)
	- #Math/discrete/graph/theorem Any subgraph of a planar graph is also a planar 
	- #Math/discrete/graph/theorem Merging two adjacent vertices of a planar graph leaves another planar graph 
	- [[Tree]] is also planar graph
- A planar can be splits into **regions**
	- ![|200](https://media.geeksforgeeks.org/wp-content/uploads/planar-regions.jpg)
	- each region is the space between edges
	- also count the outer region

### Euler's formula:
- Let $G$ be a connected planar simple graph with $e$ edges and $v$ vertices. 
- Let $r$ be the number of regions in a planar representation of $G$
- Then $\color{tomato}r=e-v+2$ 
- Corollary 1: 
	- #Math/discrete/graph/theorem If $G$ is a connected planar simple graph, with $e$ edges and $v$ vertices, where $v\ge 3$
	- then $e\le 3v-6$ 
- Corollary 2:  
	- #Math/discrete/graph/theorem If 𝐺 is a connected planar simple graph
	- then 𝐺 has a vertex of $deg \le 5$
- Corollary 3: 
	- #Math/discrete/graph/theorem If a connected planar simple graph has 𝑒 edges and 𝑣 vertices with 𝑣 ≥ 3 and no circuits of length three
	- then $e\le 2v-4$
<!--ID: 1708098041694-->

### Homeomorphic:
- #Math/discrete/graph/theorem  The graph $G_1=(V_1,E_1)$ and $G_2=(V_2,E_2)$ are called **homeomorphic** if they can be obtained from the same graph by a sequence of **elementary subdivisions**
	- [[Elementary Subdivision]] is when remove an edge $\{u,v\}$  and add new vertex $w$ together with edge $\{u,w\}$ and $\{w,v\}$
	- ![|250](https://i.imgur.com/dAELX5A.png)
<!--ID: 1708098041698-->


### Non planar
- #Math/discrete/graph/theorem A graph is non-planar IFF it contains a subgraph Homeomorphic to $K_{5}$ or $K_{3,3}$
	- ![250](https://www.researchgate.net/publication/257878116/figure/fig9/AS:302583018213413@1449152821929/Auxiliary-graphs-in-Kuratowski-theorem-a-K5-and-bK3-3.png)
<!--ID: 1708098041702-->
