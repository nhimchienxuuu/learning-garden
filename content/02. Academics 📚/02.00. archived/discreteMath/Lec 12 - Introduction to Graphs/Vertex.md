---
tags:
  - Math/discrete/graph
aliases:
  - Node
  - node
  - vertices
---
# Vertex
### Description:
- End point
### Adjacent vertices:
- Two vertices 𝑢 and 𝑣 in an ==undirected== graph 𝐺 are called adjacent (or neighbors) in 𝐺 if 𝑢 and 𝑣 are endpoints of an edge 𝑒 of 𝐺. 
- Such an edge 𝑒 is called incident with the vertices 𝑢 and 𝑣 and 𝑒 is said to connect 𝑢 and 𝑣.
<!--ID: 1708098041595-->

### Neighborhood, $N(v)$:
- The set of all neighbors of a vertex 𝑣 of 𝐺 = (𝑉, 𝐸), denoted by 𝑁(𝑣), is called the neighborhood of 𝑣. 
- If 𝐴 is a subset of 𝑉, we denote by 𝑁(𝐴) the set of all vertices in 𝐺 that are adjacent to at least one vertex in 𝐴. So, $𝑁 (𝐴) = \cup_{v\in A} 𝑁(𝑣)$ 
<!--ID: 1708098041601-->

### Degree of a vertex, $deg(v)$:
- The degree (or valency) of a vertex in an undirected graph is the number of edges incident with it
	- except that a loop at a vertex contributes twice to the degree of that vertex. 
- Pendant: vertex with degree 1
- Isolate: degree o vertex
<!--ID: 1708098041605-->
