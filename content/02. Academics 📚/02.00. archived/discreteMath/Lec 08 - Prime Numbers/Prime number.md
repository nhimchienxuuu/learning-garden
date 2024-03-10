---
mindmap-plugin: basic
tags:
  - Math/discrete/definition
aliases:
  - prime
---
# Prime number

## Description:
- Let $p\in \mathbb N$ and $p>2,p$ is **prime** if its only positive divisors are 1 and $p$
- Otherwise, $p$ is composite, there exists $a$ such that $1<a\le \sqrt p$ and $a|p$ #Math/discrete/theorem

## The fundamental of theorem of arithmetic:
- Every natural number $n>1$ can be **uniquely factored** into a product of a sequence of non-decreasing primes, i.e. the **unique prime factorization** #Math/discrete/theorem
- Euclid theorem: there are infinitely many primes #Math/discrete/theorem
<!--ID: 1708098041440-->


## Prime number theorem:
- Let $\pi(N)$ be the number of primes $\le N$. Then:$$\lim\limits_{N\to \infty}\frac{\pi(N)}{N/\ln N}=1$$
<!--ID: 1708098041444-->


## Relative primality:
- Two positive integers $a,b\in \mathbb N^+$ are relatively prime (or co-prime) if $gcd(a,b)=1$ #Math/discrete/definition
	- Prime to each other
- Two positive integers $a,b\in \mathbb N^+$ are [[#Relative primality math/discrete/definition|relatively prime]] if and only if there exists $s,t\in\mathbb Z$ such that $sa+tb=1$ #Math/discrete/theorem
	- [[Extended Euclidean algorithm]] with prime number
- If $a$ and $b$ are relatively prime and $a|bc$, then $a|c$ #Math/discrete/lemma
<!--ID: 1708098041447-->


## Pairwise relatively prime:
- The integers $a_{1,}a_{2},...,a_{n}$ are pairwise relatively prime if $gcd(a_{i}, a_{j}) =1$ whenever $1\le i<j\le n$ #Math/discrete/definition
- If integers $a_1,a_{2},...,a_{n}$ are pairwise relatively prime, then $gcd(a_{1}.a_{2}.....a_{k+1})=1$ for all $k=1,2,...,n-1$ #Math/discrete/lemma
- If integers $a_{i},a_{2},...,a_{n}$ are pairwise relatively prime, and $a_k|m$ for all $k=1,2,...,n$ and some integer $m$ then $a_{1}.a_{2}....a_{n}|m$ #Math/discrete/theorem
	- If each of the prime divides $m$ then their product also divides $m$
<!--ID: 1708098041449-->


## Least common multiple:
- The least common multiple of the positive integers $a$ and $b$ is the smallest positive integer that is divisible by both $a$ and $b$, denoted by $lcm(a,b)$ #Math/discrete/definition
- Let $a$ and $b$ be positive integers. Then $ab=gcd(a,b)\cdot lcm(a,b)$ #Math/discrete/theorem
<!--ID: 1708098041453-->


## Multiplicative inverse:

^d91a8b
<!--ID: 1708098041457-->


- Let $a,b\in \mathbb N^+$. There exist an element $a^{-1}$ such that $a^{-1}\cdot a\equiv 1(\mod b)$ if and only if $a$ and $b$ are relatively prime. #Math/discrete/theorem
	- Solutions are not unique, some may not have solution
	- Inverse of a [[Multiplication modulo|modulo]] ^4c9b7a

## Primality
- If $p$ is prime and $p\big| \Pi_{i=1}^{n}a_i$, then there exist some $1\le j\le n$ such that $p|a_j$ #Math/discrete/lemma
	- If a prime divides a product of $n$ numbers, then that prime divides at least 1 of the numbers
<!--ID: 1708098041461-->
