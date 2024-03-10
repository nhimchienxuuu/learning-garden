---
mindmap-plugin: basic
time: 2023-12-25T15:34:00
tags: []
source: https://vinuni.instructure.com/courses/1727/files/280671?module_item_id=69659
content: dyad, sum of dyads, SVD theorem
nextstep:
---
# Dyads
### Definition of dyads
- Dyad: Matrix $A \in \mathbb{R}^{m,n}$ that can be written in the form $A=p q^T$
	- $p \in \mathbb{R}^{m}$, $q \in \mathbb{R}^{n}$
	- interpretation: [here](https://i.imgur.com/yK9LiUE.png)
- Individual element: $A_{ij} = p_i.q_j$
	- $A_{ij}$ is the element in the (i)th row and (j)th column of the matrix A
	- $p_i$: i-th element of p, $(1 \leq i \leq m)$
	- $q_j$: j-th element of q, $(1 \leq j \leq n)$
- Interpretation: 
	- the columns of p are scaled, by a scaling factor given in vector q, and result in the columns in A
	- the rows of $q^T$ are scaled, by a scaling factor given in vector p, and result in the rows in A
- Examples of video frames
	- a set of image frames representing a video, each image represented by a row vector of pixels -> can represent the whole video as a matrix A
	- if the video shows a no-movement scene 
	  -> each row in matrix A is identical 
	  -> all rows are scaled copies of the same row vector + all cols are scaled copies of the same col vector 
	  -> matrix A is dyad
<!--ID: 1708098042348-->

### Sum of dyads
- SVD theorem: any matrix can be written as a sum of dyads: $A=\sum_{i=1}^{r}p_{i}q_{i}^{T}$ ($p_i, q_i$ are mutually orthogonal)
- can interpret data as sum of simpler matrix (dyads)
- mutual orthogonality of each dyad ensures each encodes independent information
<!--ID: 1708098042351-->
