---
mindmap-plugin: basic
time: 
tags: 
source:
---
# norms and lp norms
### norm
- a real-valued function maps and $x \in R^n$ into a real number
- denote: $||x||$, norm = length of the vector (vector of norm 1 = unit vec)
- $||x||$ is a norm if:
	- $\|x\|\geq0\ \forall x\in X, ||x|| = 0$ IFF $x = 0$
	- $\|x+y\|\leq\|x\|+\|y\|,$ for any $x, y \in X$  (triangle inequality)
	- $||\alpha x|| = |\alpha|.||x||$, for any $\alpha$ scalar and $x \in X$
<!--ID: 1708098042596-->


### lp norms
- defined as $\|x\|_{p}\doteq\left(\sum_{k=1}^{n}|x_{k}|^{p}\right)^{1/p},\quad1\leq p<\infty$
- p = 2: standard Euclidean length
	- $\|x\|_{2}\doteq\sqrt{\sum_{k=1}^{n}x_{k}^{2}}$
- p = 1: sum-of-absolute-values length
	- $\|x\|_{1}\doteq\sum_{k=1}^{n} |x_{k}|$ 
- p = $\infty$: max absolute value norm / Chebyshev norm
	- $\|x\|\infty\doteq\operatorname*{max}_{k=1,\ldots,n}|x_{k}|$
- p = 0: pseudo norm / the cardinality (number of non-zero elements) / $\ell_{p}$ 
<!--ID: 1708098042601-->


### unit balls associated with popular lp norms
- ![](https://i.imgur.com/pTlUVRR.png)
- $I_2$ measures ordinary distance
- $I_1$ measures distance in a rectangular grid
- $I_\infty$ measures peak (absolute) values
<!--ID: 1708098042605-->
