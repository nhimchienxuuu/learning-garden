---
mindmap-plugin: basic
tags:
  - Math/discrete/definition
---
# Euclid & GCD algorithm
### Description:
- 
  ```python
  def EuclidAgl(a,b):
	  if b = 0:
		  return a
	  else:
		  return EuclidAlg(b, a mod b)
	```
	- If $a,b\in \mathbb N, b\not=0$ then $gcd(a,b)= gcd(b, a\mod b)$ #Math/discrete/lemma
- Euclid’s algorithm, on input EuclidAlg(a, b) for $a, b ∈ N^+, a, b$ not both 0, always terminates and produces the correct output. #Math/discrete/theorem 
- For every two recursive calls made by EuclidAlg, the first argument a is at least reduced by halved. #Math/discrete/claim 
- #Math/discrete/theorem Euclid’s algorithm, on input EuclidAlg(a, b) for $a, b ∈ N+$, a, b not both 0, always  terminates in time proportional to $log_2a$
	- if a larger, algorithm increase logarithmically, not linearly 
### Theorem 11 (Bézout Theorem)
- Let a, b ∈ N+, a, b not both 0. Then, there exist s, t *(Bézout coefficients)* ∈ Z such that $sa + tb = gcd(a, b)$ *(Bézout identity)*
- How to compute $s,t$ from $gcd(a,b) = z$
	- write out a = b.q + r for each recursive call (from $r_1$ -> $r_n$ , for eg) of solving EuclidAlg(a, b), until there is no remainder left
	- writing in backward order, from z = elements of $r_1$ -> $r_n$
	- compute so that you get the form $sa + tb = z$
<!--ID: 1708098041351-->


