---
mindmap-plugin: basic
time: 
tags: 
source:
---
# relations - discrete math
## Relation description
### Def 1:
- a binary relation R consists
	- set A: domain of R
	- set B: codomain of R
	- subset of A x B: graph of R
- example:
	- A = {1,2} 
	- B = {a,b,c},
	- R = {(1,a),(1,b),(2,c)} is a relation from A to B, or a subset of A x B
- note:
	- $R: A -> B$: R is a relation from A to B
	- "$a\;R\;b$": the pair (a, b) in the graph of R
- confusing example:
	- [[Pasted image 20231125224048.png|eg1]]
<!--ID: 1708098041104-->


## Relation Types:
### Reflexive, Symmetric, Transitive
- A relation R on set S is:
- Reflexive: 
	- every element in S is related to itself
	- if $(x, x) \in R$ for all $x \in S$
	- eg: the "equal" relation is reflexive, as every number is equal to itself
	- *tips*: is x "the relation" to x correct
- Symmetric:
	- order of elements in the pair don't matter
	- $(x,y) \in R$, then $(y,x) \in R$
	- eg. the "is sibling of relation is symmetric" as if x is sibling of y, then y is also sibling of x
- Transitive: (suy ra)
	- if x related to y, y related to z, then x is also related to z
	- if $(x,y) \in R$, and $(y,z) \in R$, then $(x, z) \in R$
<!--ID: 1708098041108-->


### Inverse relation
- $R^{-1}$ of $R: A \to B$ is the relation from B to A defined by $(b\;R^{-1}\;a)\;\; IFF\;\;(a\;R\;b)$ 
- change the position & reverse arrow sign: $A \to B$ into $B \to A$ 
<!--ID: 1708098041113-->
