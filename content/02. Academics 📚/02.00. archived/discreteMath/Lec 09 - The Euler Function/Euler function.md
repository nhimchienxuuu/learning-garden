---
mindmap-plugin: basic
tags:
  - Math/discrete
---

# Euler function: $\phi$

## Euler function $\phi$:
- Given a positive integer $n\in \mathbb N^+$, define $\phi(n)$ to be the number of integers $x\in \mathbb N^{+},x\le n$ such that $gcd(x,n)=1$
	- number of integers that are [[Prime number#Relative primality|relatively prime]] with $n$. ==1== is also counted
	- $\phi(6)=2, \phi(7)=6$
- If the prime factor of $n$ is $n=p_{1}^{k_{1}}.p_{}^{k_{2}}...p_{m}^{k_{m}}$ then #Math/discrete/theorem $$\phi(n)=n\prod\limits_i\bigg(1-\frac{1}{p_{i}}\bigg)=\prod_i\bigg(p_{i}^{k_{i}}-p_{i}^{k_{i}-1}\bigg)$$
- If $p$ is a prime, then ${\color{tomato}\phi(p)=p-1}$. If $n=pq$ where $p\not= q$ are both primes, then $\color{tomato}\phi(n)=(p-1)(q-1)$ #Math/discrete/corollary
	- $n$ is composite
<!--ID: 1708098041476-->


## [[Euler's theorem]]
## [[Primality test]]