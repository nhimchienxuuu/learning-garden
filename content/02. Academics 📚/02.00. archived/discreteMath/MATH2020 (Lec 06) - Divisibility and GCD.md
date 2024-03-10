---

mindmap-plugin: basic

---
# Divisibility and GCD

## Number Theory
- study of integers, that is set $\mathbb{Z}$
- study Cryptography - secure communication, privacy, e-commerce
- cryptocurrency
<!--ID: 1708098041897-->


## Divisibility
### Def 1: Divisibility
- Let $a, b \in \mathbb{Z}, a \ne 0$
- a divides b, denoted by $a | b$, if there exists some $k \in \mathbb{Z}$ such that $ak = b$
- $3 . 4 = 12$, $3 | 12$ (k = 4), $12 : 3$
<!--ID: 1708098041902-->


### Theorem 2:
- Let $a, b, c \in \mathbb{Z}$
	- $a|b$ and $a|c$ then $a | (b+c)$ or $a | (b-c)$
	- $a|b$ then $a | bc$
	- $a|b$ and $b|c$ then $a|c$ (i.e. transitivity)
<!--ID: 1708098041906-->

### Corollary 3:
- Let $a, b, c \in \mathbb{Z}$. If $a|b$ and $a|c$, then $a|(mb+nc)$ for any $m,n \in \mathbb{Z}$
<!--ID: 1708098041910-->


## Division Algorithm
### Theorem 4
- For any $a \in \mathbb{Z}$ and $d \in \mathbb{N^+}$, there exist unique $q,r \in \mathbb{Z}$ such that $a = dq + r$ and $0 \leq r < d$
<!--ID: 1708098041916-->

### Definition 5
- In this equation, $a = dq + r$,
- d: divisor, a: dividend.
- q is called the quotient, denoted by q = a div d .
- r is called the remainder, denoted by r = a mod d.
<!--ID: 1708098041922-->


## Greatest Common Divisor
### Definition 6 (GCD)
- $a,b \in \mathbb{Z}$ with a, b not both = 0. $gcd(a,b)$ is largest integer d such that $d|a$ and $d|b$
- Note: $gcd(n,m) = gcd(m,n)$
- $a = gcd(a, b) * m$, $b = gcd(a, b) * n$, where $gcd(m,n) = 1$
<!--ID: 1708098041927-->


## Euclid Algorithm
### Lemma 7: 
- for reducing the problem of finding gcd of 2 large numbers to smaller ones
- $a, b \in \mathbb{N}, b \neq 0$, $gcd(a,b) = gcd(b,\;a\;mod\;b)$
	- recursive $a-b$ is just like finding remainder of $a / b$
<!--ID: 1708098041930-->


- 
  ``` python
  if b=0:
	  return a;
  else
	  return EuclidAlg(b,a mod b);
  ```

### Theorem 8
- Euclid’s algorithm (EuclidAlg), on input EuclidAlg(a, b) for $a, b ∈ N+$, $a, b$ not both 0, always terminates and produces the correct output
<!--ID: 1708098041935-->

### Claim 9
- For every two recursive calls made by EuclidAlg, the first argument a is at least reduced by halved
<!--ID: 1708098041940-->


### Theorem 10
- Euclid’s algorithm, on input EuclidAlg(a, b) for $a, b ∈ N+$, a, b not both 0, always  terminates in time proportional to $log_2a$
	- if a larger, algorithm increase logarithmically, not linearly
<!--ID: 1708098041943-->


### Theorem 11 (Bézout Theorem)
- Let a, b ∈ N+, a, b not both 0. Then, there exist s, t *(Bézout coefficients)* ∈ Z such that $sa + tb = gcd(a, b)$ *(Bézout identity)*
- How to compute $s,t$ from $gcd(a,b) = z$
	- write out a = b.q + r for each recursive call (from $r_1$ -> $r_n$ , for eg) of solving EuclidAlg(a, b), until there is no remainder left
	- writing in backward order, from z = elements of $r_1$ -> $r_n$
	- compute so that you get the form $sa + tb = z$
<!--ID: 1708099388779-->


### Extended Euclidean Algo ❓❓❓
![|300](https://i.imgur.com/K7mwiH7.png)
$q_{i+1} = r_0/r_1$
<!--ID: 1708098041948-->

