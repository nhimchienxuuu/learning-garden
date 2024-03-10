---

mindmap-plugin: basic

---
# Functions and Relations
## Relations:
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
<!--ID: 1708099388780-->


## Relation Types:
### Def 2 (Reflexitivity, symmetry, transitivity)
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
<!--ID: 1708098041813-->


### Def 3 (Functions) ❓❓❓
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
<!--ID: 1708098041819-->


### Def 4 (Injection / One-to-one)
- a function $f: S \to T$ is "injective" if for every $t \in T$, there exists AT MOST one $s \in S$ such that $f(s) = t$
- one output is mapped to AT MOST one input
- <u>prove</u>: 
	- assume $f(x_1) = f(x_2)$ for $x_1, x_2$ in S 
	- show that this implies $x_1 = x_2$
<!--ID: 1708098041823-->


### Def 5 (Surjection / Onto) ❓❓❓
- a function $f: S \to T$ is "surjective" (onto) if the image of f equals its range, or for each $t \in T$, there is AT LEAST one $s \in S$ such that $f(s) = t$
- <u>prove</u>: 
	- let f(s) = t => s = ...
	- as $t \in T$, if $s \in S$ -> surjective
<!--ID: 1708098041827-->


### Def 6 (Bijection / One to one correspondence)
- a function $f: S \to T$ is "bijective" if it is injective and surjective
- every element of the codomain corresponds to exactly one element of the domain
<!--ID: 1708098041831-->


## Function Composition & Inverse
### Def 7 (Composition)
- for $f: A \to B$ and $g: B \to C$
- $g \circ f = g(f(x))$
- $f \circ g = f(g(x))$
- $g \circ f \neq f \circ g$, if well defined
<!--ID: 1708098041838-->


### Inverse relation
- $R^{-1}$ of $R: A \to B$ is the relation from B to A defined by $(b\;R^{-1}\;a)\;\; IFF\;\;(a\;R\;b)$ 
- change the position & reverse arrow sign: $A \to B$ into $B \to A$ 
<!--ID: 1708099388781-->


### Def 9: identity function
- identity function is a function returning the same output as its input
- $id_A: A \to A$ - a function maps set A to itself
- eg
	- A is set of real numbers
	- $x \in A$, $id(x) = x$; for eg $x = 5$, then $id(5) = 5$
- <u>prove</u>
	- for every x in domain f, $f(x) = x$
<!--ID: 1708098041846-->


### Def 10: left / right inverse
- $f \circ g = id$ => f is left inverse of g, g is right inverse of f
<!--ID: 1708098041851-->


### Def 10: two-sided inverse
- f is both left and right inverse of g -> f and g are two sided inverses of each other
<!--ID: 1708098041856-->


### Def 12:
- f from A to B is **total** when f(x) exists for all $x\in A$
<!--ID: 1708098041864-->


### Claim 13, 14, 15: work for both sides
- f is **injective** and total <=> f has **left inverse**
- f is **surjective** <=> f has **right inverse**
- f is **bijective** <=> f has a **two-sided inverse**
<!--ID: 1708099388782-->


## Set cardinality 
- [[MATH2020 (Lec 01) - Set Theory#^e542b3|review definition in lec 1]]
- set cardinality: number of elements in a set, either finite or infinite
- Two sets $A$ and $B$ have the same cardinality (written as $|A| = |B|$) IFF there exists a bijection $f: A \to B$
- Set $A$ has cardinality $\geq$ set $B$ (written as $|A| \geq |B|$ ) IFF there exists 
	- an injection $g: A \to B$
	- a surjection $g': B \to A$
<!--ID: 1708098041869-->


## Set countability
### Countable & Uncountable Set
- countable if it has same number of elements as some subset of $\mathbb{N}^+$ or $\mathbb{N}^+$ itself
- include finite and infinite set that is **bijective** with $\mathbb{N^+}$
- a set is countable IFF $|S| ≤ |N^+|$
- eg: 
	- set $\mathbb{Z}$ is also countable: alternating between non-negative and negative numbers -> [[Pasted image 20231126161402|here]]
- prove S is countable set:
	- find a bijection between the set S and $\mathbb{N^+}$
- a set not countable is uncountable
	- *Proposition 2*: eg. set of (0, 1); $\mathbb{R}$ is uncountable
<!--ID: 1708099388783-->


### Cantor-Bernstein-Schroeder
- if $f: S \to T$ is injective (or $|S| \leq |T|$) and $g: T \to S$ (or $|T| \leq |S|$) is injective => there is a bijective $h: S \to T$
<!--ID: 1708099388784-->


### Theorem 18
- if A and B are countable sets, $A \cup B$ is also countable
<!--ID: 1708099388785-->


## Rational and irrational numbers
- *rational numbers*: any number expressed as the fraction $\frac{p}{q}$ with p, q are integers 
- *irrational numbers*: real number that cannot be expressed as fraction of 2 int (eg. pi, e, sqrt(2))
<!--ID: 1708098041881-->


![[Pasted image 20231129223906.png]]