---
mindmap-plugin: basic
time: 
tags: 
source:
---
# title
### description
- Common set operations
	- Union: $S \cup T = \{x | x \in S \lor x \in T\}$: elements in S or T
		- $\lor$: or
	- Intersection: $S \cap T = \{x | x \in S, x \in T\}$: intersection of S and T only
	- Differences: $S - T = \{x | x \in S, x \notin T\}$: in S but not T
	- [[Pasted image 20231124143245.png|Complements]]: $\overline{S} = \{x | x \in \mathbb{U}, x \notin S\} = \mathbb{U} - S$
		- $\mathbb{U}$ is the universe containing sets S and T
- Theorem 15
	- For all sets S and T, $S = (S \cap T) \cup (S - T)$
	- **Prove Set Equality**: show that $S \subset (S \cap T) \cup (S - T)$ and $(S \cap T) \cup (S - T) \subset S$
	- see the prove [[Pasted image 20231124143544.png|here]]