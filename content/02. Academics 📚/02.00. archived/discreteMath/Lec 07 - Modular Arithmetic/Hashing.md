---
mindmap-plugin: basic
time: 
tags: 
source:
---
# title
### Application of [[Arithmetic modulo|Arithmetic modulo - Discrete Math]] - Hashing
- hashing: $h(k) = k\;mod\;N$
- Pseudo random sequences: use the linear congruential generator (LCG) to generate
	- choose 4 int: modulus m, multiplier a, increment c, seed $x_0$, $2 \leq a < m$, $0 \leq c < m$, $0 \leq x_0 < m$
	- $x_{0} = random\;seed$
	- $x_{i} = (a \cdot x_{i-1} + c) \mod m$
<!--ID: 1708098041418-->
