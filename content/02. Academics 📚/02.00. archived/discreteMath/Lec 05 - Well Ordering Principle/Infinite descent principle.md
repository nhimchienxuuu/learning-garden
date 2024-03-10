---
mindmap-plugin: basic
tags:
  - Math/discrete/definition
aliases:
  - Fermat's method of descent
---
# Infinite descent principle
### Description
-  There is no infinite sequence of strictly decreasing non-negative integers #Math/discrete/theorem 
- Used to show that a statement cannot possibly hold for any number
	- by showing that if the statement were to hold for a number
	- then the same would be true for a smaller number
	- leading to an infinite descent and ultimately a contradiction.
- The method relies on [[Well ordering principle]], so only a finite number of non-negative integers are smaller than any given one
- A method of [[Proof by contradiction]]
- Used to solve [[Fermat's Last Theorem for n = 3, 4]]
<!--ID: 1708098041209-->

### Proof by contradiction
- Let P is a property for nonnegative integers
- Assume P(0) is true
- for all $k \in \mathbb{N}$, if $P(k)$ is false, there exist an $m < k$ that $P(m)$ is also false -> contradicting to the WOP
- Then, $P(n)$ is true for all $n \in \mathbb{N}$, including $k$
- <u>Example</u>: 
	- P(n): “n is a positive integer that is not divisible by any square number other than 1”
	- assume there exists a k satisfies P(n)
	- k is not divisible by any square number other than 1. 
	- but every positive number is divisible by 1^2 (which is 1) -> there exists a smaller number m where m = k/ 1^2 = k satisfies P(n). 
	- but this is still k and we are not actually finding a new number, contradicts that we could keep finding a smaller numbers satisfies P, leading to infinite descent
- <u>Core situation:</u> 
	- we can keep finding smaller and smaller natural numbers violating a property >< in a set of natural numbers, there is a smallest element (WOP)
	- if $P(k)$ is true, there will be $P(m)$ and infinite descent numbers of $m$, contradicting with the WOP
<!--ID: 1708098041212-->
