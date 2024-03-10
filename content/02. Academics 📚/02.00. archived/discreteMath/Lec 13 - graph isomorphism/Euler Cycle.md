---
tags:
  - Math/discrete/graph
---
# Euler Cycle
### Description:
- A cycle that **uses every edges in a graph exactly once**
- A undirected graph 𝐺 = (𝑉, 𝐸) has an Euler cycle if and only if 𝐺 is **connected** and every 𝑣 ∈ 𝑉 has **even degree**. #Math/discrete/graph/theorem  
- A directed graph 𝐺 = (𝑉, 𝐸) has an Euler cycle if and only if 𝐺 is strongly **connected** and every 𝑣 ∈ 𝑉 has **equal in-degree and out-degree**. #Math/discrete/graph/theorem 
- Constructing Euler circuit:
	- Start from any vertex and find a sub-cycle, start and end at this vertex (it exists due to the even degrees assumption)  
	- Remove all edge of this sub-cycle.  
	- Repeat the process at an appropriate vertex until all edges were removed.  
	- Combine the sub-cycles to form the Euler cycle.  
