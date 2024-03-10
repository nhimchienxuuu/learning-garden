---
mindmap-plugin: basic
time: 
tags: 
source:
---
# affine
### definition
- of the form $A=\{x\in X:x=v+x^{(0)},\,v\in{\mathcal{V}}\}=x^{(0)}+{\mathcal{V}}$
	- $\mathcal{V}$ is subspace of X
	- obtained by adding a single vector to the span of a set of vectors
- [[subspace and span|Subspace]] are just affine space containing the origin, but not necessary have to pass through it
<!--ID: 1708098042393-->


### linear and affine functions
- a function f is affine IFF the function $f(x) = a^Tx+b$ is linear, for some unique pair (a,b); $a \in R^n$ and $b \in R$
- function is linear IFF $b = 0$
- affine = linear + constant
- difference btw a linear function & affine function: 
	- a linear function **always passes through the origin**
	- affine function does not necessarily do so
- find a and b:
	- $a_i = f(e_i) - b$ with $e_i$ is the $i-th$ unit vector
	- $b = f(0)$
<!--ID: 1708098042396-->

### linear map
- $a \in R^n$ can be viewed as linear map from input space $R^n$ to output space $R$
<!--ID: 1708098042400-->
