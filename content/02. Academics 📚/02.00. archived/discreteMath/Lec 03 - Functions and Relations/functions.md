---
mindmap-plugin: basic
time: 
tags: 
source:
---
# title
### description
- a function $f: S \to T$ is a mapping from set S to elements in set T, to which each element in 1 set (domain set) is mapped to exactly 1 element in another set (codomain set)
- $f: S \to T$
	- f: function
	- S: domain
	- T: codomain
	- f is a relation between S and T. For each $s$ in S there is a unique element $t$ in T so that $(s, t) \in R$
	- image / range of $f$ is set of all values $f$ can produce
- note:
	- *image*: set of output that the function actually produce <u>for a particular input</u>
	- *range*: set of output that the function could produced, eh

### types of function
- [[injection]]
- [[surjection]]
- [[bijection]]
<!--ID: 1708098041059-->


### Def 7 (Function Composition)
- for $f: A \to B$ and $g: B \to C$
- $g \circ f = g(f(x))$
- $f \circ g = f(g(x))$
- $g \circ f \neq f \circ g$, if well defined
<!--ID: 1708098041065-->


### identity function
- identity function is a function returning the same output as its input
- $id_A: A \to A$ - a function maps set A to itself
- eg
	- A is set of real numbers
	- $x \in A$, $id(x) = x$; for eg $x = 5$, then $id(5) = 5$
- <u>prove</u>
	- for every x in domain f, $f(x) = x$
<!--ID: 1708098041068-->


### left / right inverse
- $f \circ g = id$ => f is left inverse of g, g is right inverse of f
<!--ID: 1708098041072-->


### two-sided inverse
- f is both left and right inverse of g -> f and g are two sided inverses of each other
<!--ID: 1708098041077-->


### total function
- f from A to B is **total** when f(x) exists for all $x\in A$
<!--ID: 1708098041082-->


### Claim 13, 14, 15: work for both sides
- f is **injective** and total <=> f has **left inverse**
- f is **surjective** <=> f has **right inverse**
- f is **bijective** <=> f has a **two-sided inverse**
<!--ID: 1708098041086-->


### Cantor-Bernstein-Schroeder
- if $f: S \to T$ is injective (or $|S| \leq |T|$) and $g: T \to S$ (or $|T| \leq |S|$) is injective => there is a bijective $h: S \to T$
<!--ID: 1708098041090-->
