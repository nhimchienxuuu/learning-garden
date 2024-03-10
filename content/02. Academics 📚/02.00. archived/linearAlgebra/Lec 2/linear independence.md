---
mindmap-plugin: basic
time: 
tags: 
source:
---
# linear independence
### linear dependent
- the state that a vector can be written by other vectors
- eg. we have $a,b,c$ are vectors; $c = a + 2b$; => $2a + b - c = 2a + b - (a+2b)$
  => a, b, c are linearly dependent
<!--ID: 1708098042454-->


### linear independent
- none of the vectors can be written in terms of other vectors 
- require that the [[linear combination]] equation is equal to $\vec{0}$ when all scalars are equal zero
	- A: $c_1 \vec{v_1} + c_2 \vec{v_2} + \cdots + c_n \vec{v_n} = \vec{0}$ 
- check independence (normal, slow way)
	- find a valid set of nonzero scalars ($c_1 \; to\;c_n)$ satisfying A
		- if possible -> linear dep
		- if impossible -> linear indep
<!--ID: 1708098042458-->


### prove linear independence
- Way 1: (elementary row operations) find scalars to see whether all of them = 0 when scalars = 0
	- just like in *check independence* above
- Way 2: row echelon
	- do elementary row operations so that diagonal matrix have diagonal value of 1, the below diag of 0.
	- if after construction -> REF is 100% match or u cannot write any vector in terms of the other -> linear indep
	- ![](https://i.imgur.com/oJiRPQT.png)
	- ![](https://i.imgur.com/1ssXRwO.png)
<!--ID: 1708098042461-->


- Way 3: finding [[determinant]] (sqr matrix only)
	- if zero -> linear dep
	- if nonzero -> linear indep