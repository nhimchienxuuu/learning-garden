---

mindmap-plugin: basic

---

# Set Theory
## set definition
- **unordered** collection of **distinct** objects
	- eg. $V = \{u, e, o, a, i\}$
- set builder notation: $P = {x\in \mathbb{Z}^+ |\; x\;is\;prime\;number\;and\;x < 20}$
- data types in CS is built upon the concept of a set
- 
  ```python
    my_set = {1,2,"hi"}
	# set from iterable object
	my_set = set([1,2, "hi"])
	```
- 
	```java
	  Set<Integer> mySet = newHashSet<>();
	```
<!--ID: 1708098041220-->


## Equal Set
- every element in 1st set is in 2nd set, and vice versa $\forall x (x \in A \leftrightarrow x \in B)$
- **Remark 1:** empty set / null set is special set with no element $\emptyset$
- **Remark 2:** set with 1 element: *singleton set*
<!--ID: 1708098041224-->

## Subset:
- A is a subset of B, and B is a superset of A <=> every element of A is also element of B
- (A is subset of set B: $A \subseteq B$) = (B is superset of set A: $B \supseteq A$)
- **Theorem 4:** For every set S, (i) $\emptyset \subseteq S$, (ii) $S \subseteq S$
- **Remark 1**: A is proper subset of B if (i) A is a subset of B (ii) $A \neq B$
- **Remark 2:** $A \subseteq B$ and $B \subseteq C$ => $A = B$
<!--ID: 1708098041228-->


## Power Set:
- power set of S is set of all subsets of set S, $\mathcal{P}(S)$
<!--ID: 1708098041232-->


## Cardinality:

^e542b3
<!--ID: 1708098041236-->


- If have exactly n distinct elements in set S, n is nonnegative integer -> S is a finite set, n is cardinality (number of elements) of S (denoted as $|S|$)
- $\mathcal{P}(\{0, 1, 2\}) = \{\emptyset, \{0\}, \{1\}, \{2\}, \{0, 1\}, \{1, 2\}, \{0, 2\}, \{0, 1, 2\}\}$

## Ordered n-tuples
- represent ordered collection - with tuple $(a_1, a_2, ..., a_n)$
	- as this is ordered, $(1,2) \neq (2,1)$
	- $(a_1, a_2, ..., a_n) = (b_1, b_2, ..., b_n)$ <=> $a_i = b_i$ for all $i = 1,2,...,n$
<!--ID: 1708098041242-->


## Cartesian Product
- A x B, is set of all ordered pairs (a, b), where $a \in A$ and $b \in B$
$A \times B = \{(a, b) | a \in A \land b \in B\}$
	- $\land$: and
- pairs every element of the first set with every element of the second set
- eg:
	- $A = \{1, 2\}, B = \{x, y\}$
	- $A × B = \{(1, x), (1, y), (2, x), (2, y)\}$
<!--ID: 1708098041246-->


## Set operations
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
<!--ID: 1708098041254-->


## Strings
- Given a set $S$ and a natural number $n \in N$,
- $S^n$ is the set of length $n$ ‘strings’. Can be defined as product of $n$ copies of $S$ (i.e., $S \times S \times \cdots \times S$).”
	- $\{0, 1\}^n$: set of all n-bit strings. $n = 3$ -> set is all possible combination of 0 and 1 in string of length 3
	- There are $2^n$ possible strings (8 when n = 3 above)
- $S^*$ is the set of finite length ‘strings’$S^* = S^0 \cup S^1 \cup S^2 \cup ...$, where $S^0$ contains empty string.”
	- $\{0, 1\}^*$: set of all finite-length bit strings. $*$ = any length, even 0. -> set is all possible combinations of 0 and 1 for all possible lengths, including "", "0", and so on
- $[n]$ is the set $\{0, 1, 2, \cdots, n-1\}$
<!--ID: 1708098041260-->


## Russell's Paradox
- $R = \{ S | S \notin S \}$, that is R is the set of all sets that don't contain themselves as an element
- see more [[Pasted image 20231124145225.png|here]]
<!--ID: 1708098041267-->

