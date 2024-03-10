---

mindmap-plugin: basic

---
# Prime Numbers

## Private key Cryptosystems

^525a2e
<!--ID: 1708098041976-->


- refer to [[Pasted image 20231123212854.png |this pic]]
## Public key Cryptosystems

^f2413c
<!--ID: 1708098041981-->


- two keys: pub for encrypting, pri for decrypting
- Alice generate both keys by herself, give the pub to Bob to encrypt, only Alice can decrypt and read secret using her pri key
- Solution for this: RSA Algorithm
- refer to [[Pasted image 20231123213044.png |this pic]]

## Primes
### Def 1: Primes and Composites
- p ∈ N, p ≥ 2. 
	- p is prime if its only positive divisors are 1 and p. 
	- Otherwise p is composite (i.e., there exists some a such that 1 < a < n and a|n).
<!--ID: 1708098041984-->


- Primality test: How to test if a number is prime?
	- Trivial method: try to divide n by all the number between 2 and $\sqrt{n}$, inefficient considered very large 100-200 digits prime.
	- A deterministic polynomial-time algorithm to for primality tests introduced by Agarwal, Saxena and Kayal in 2002 - still practically infeasible.
	- more efficient method: probabilistic algorithm for primality test

### Theorem 2:
- If n is composite, there exist $a$ such that $1 < a \leq \sqrt{n}$ and $a | n$
<!--ID: 1708099388771-->


### Theorem 3: Fund Theorem of Arithmetic
- Every natural number $n > 1$, can be uniquely factored into a product of a sequence of non-decreasing primes, i.e., the unique prime factorization.
<!--ID: 1708098041989-->


### Theorem 4: Euclid
- There are infinitely many primes
<!--ID: 1708098041993-->


### Theorem 5: Prime Number Theorem
- $$\text{Let } \pi(N) \text{ be the number of primes } \leq N. \text{ Then}
\lim_{{N \to \infty}} \frac{\pi(N)}{N / \ln N} = 1
<!--ID: 1708098041998-->


$$

## Relative Primality / coprime
### Relative Primality / coprime
- $a, b ∈ N+$ are coprime if $gcd(a, b) = 1$.
- $a, b ∈ N+$ are coprime <=> if there exists $s, t$ ∈ $Z$ such that $sa + tb = 1$
<!--ID: 1708098042003-->


### Lemma 8:
- a and b are relatively prime, $a | bc$, then $a | c$
<!--ID: 1708098042009-->


## Pairwise Relative Primality
### Definition 9: pairwise relative prime
- The integers a1, a2, . . . , an are pairwise relatively prime if gcd (ai , aj ) = 1 whenever 1 ≤ i < j ≤ n.
<!--ID: 1708098042013-->


### Lemma 10
- $$\text{If integers } a_1, a_2, ..., a_n \text{ are pairwise relatively prime, then } \gcd(a_1 \cdot a_2 \cdot ... \cdot a_k, a_{k+1}) = 1 \text{ for all } k = 1, 2, ..., n - 1.
$$
<!--ID: 1708098042017-->

### Theorem 11: 
- If integers a1,a2,...,an are pairwise relatively prime, and ak|m for all k = 1,2,...,n and some integer m, then a1a2 . . . an|m.
<!--ID: 1708098042021-->


## Least Common Multiple
### Def 12: 
- The least common multiple of the positive integers a and b is the smallest positive integer that is divisible by both a and b. The least common multiple of a and b is denoted by $lcm(a, b)$.
- eg. lcm(5,12) = 60
- $lcm(a, b) = (a * b) / gcd(a, b)$
<!--ID: 1708099388773-->


### Theorem 13: 
- Let a and b be positive integers. Then $ab = gcd(a, b) · lcm(a, b)$
<!--ID: 1708098042026-->


## Multiplicative Inverse
### Theorem 14:
- $$\text{Let } a, b \in \mathbb{N}^+. \text{ There exists an element } a^{-1} \text{ such that } a^{-1} \cdot a \equiv 1 \; (\text{mod } b) \text{ if and only if } a \text{ and } b \text{ are relatively prime.}
$$
<!--ID: 1708098042030-->

## Primality
### Lemma 15:
- If p is prime and $\Pi_{i=1}^{n} a_i \equiv 1 \; (\text{mod } p)$, then there exists some $1 \leq j \leq n$ such that $a_j \equiv 1$
- $\Pi_{i=1}^{n}a_i$ is multiply all the terms $a_i$ for each i from 1 to n
<!--ID: 1708098042036-->

### Theorem 16 (The fundamental Theorem of Arithmetic)
- Every natural number n > 1 can be uniquely factored into a product of a sequence of non-decreasing primes, i.e., the unique prime factorization.
<!--ID: 1708098042040-->

