---
mindmap-plugin: basic
tags:
  - Math/discrete/definition
---
# Multiplication modulo
### Description:
- $a ._m b = (a · b) \mod m$
	- denoted by $._m$ 
- The operations $._m$ satisfies many of the same properties of ordinary multiplication of integers.  
	1. Closure: If $a$ and $b$ belong to $\mathbb Z_m$, then $a ._m b$ belongs to $\mathbb Zm$.  
	2. Associativity: If $a, b,$ and $c$ belong to $\mathbb Zm$, then $(a ._m b) ._m c = a ._m (b ._m c)$
	3. Commutativity: If $a$ and $b$ belong to $\mathbb Zm$, then $a ._m b = b ._m a$
	4. Identity element: The element 0 is identity element for addition modulo m. That is, if a belongs to $\mathbb Zm$, then $a ._m 1 = 1 ._m a = a$. 
	5. Distributivity: If $a, b,$ and $c$ belong to $\mathbb Z_m$, then $a ._m (b +_m c) = (a ._m b) +_m (a ._m c)$ and $(a +_m b) ._m c = (a ._m c) +_m (b ._m c)$.
- $\mathbb Z_m$ with modular [[Addition modulo operation|addition]] and multiplication is said to be a [[Commutative ring]]
- The multiplicative inverses has not been included $\mathbb Z_m$ as it may not be exists  
	- (E.g., no multiplicative inverse of 2 modulo 6).  
- For some certain value of $m$, the multiplicative inverses exists (for all element not 0), in this case, $\mathbb Z_m$ is a field.