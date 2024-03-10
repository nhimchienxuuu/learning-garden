---
mindmap-plugin: basic
tags:
  - Math/discrete/theorem
---

# Euler's theorem

## Description:
- Given $a,n\in \mathbb N^+$, if $a$ and $n$ are [[Prime number#Relative primality|relatively prime]], then $\color{tomato}a^{\phi(n)}\equiv1(mod\ n)$ #Math/discrete/corollary
- If $gcd(a,n)=1$, then $\color{tomato}a^{\phi(n)-1}\mod n$ is an [[Prime number#^4c9b7a|inverse of a modulo]] $n$ #Math/discrete/corollary ^4b2036
- If $gcd(a,n)=1$, then $a^{x}\equiv a^{x\mod\phi(n)}\mod n$ #Math/discrete/corollary
- Let $\mathbb Z^{*}_{n}=\{ k|1\le k \in \mathbb N^{+}, k\le n, gcd(k,n)=1\}$. Consequently $\phi(n)=|\mathbb Z^{*}_{n}|$ #Math/discrete/definition
	- Set of all relative prime and 1
- If $j,k\in \mathbb Z^{*}_{n}$ then $j{\color{tomato}\cdot_{n}}k\in \mathbb Z^{*}_{n}$ #Math/discrete/lemma
	- [[Multiplication modulo]]
- For any element $k$ and subset of $S$ of $\mathbb Z_{n}$, let define $kS\triangleq \{ k\cdot_{n}s\ |\ s\in S\}$ #Math/discrete/definition
	- Example: $k=3,n=10\to k\mathbb Z^{*}_{10}=\{3 \cdot_{10} 1, 3\cdot_{10} 3, 3 \cdot_{10} 7, 3 \cdot_{10} 9\}=\{3,9,1,7\}$

## [[Fermat's little theorem]]
