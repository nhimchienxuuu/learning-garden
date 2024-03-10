---
tags:
  - Math/discrete/definition
---

# Arithmetic modulo
## Definitions & Theorems:
### Definition 1
- $a, b ∈ Z, m ∈ N+$
- $a$ and $b$ are **congruent modulo** $m$ or $a ≡ b (mod\;m)$ (a congruence) if they leave the **same remainder** when divided by m (its modulus)
- $a ≡ b (mod\;m)$ if the 
difference between a and b 
is a multiple of m -> 
$m|(a − b)$ or  $a − b = km$
- a and b not congruent modulo m, we write $a \not\equiv b \; (\text{mod} \; m)$
<!--ID: 1708098041376-->


### Theorem 2
- $a$ and $b$ are int, m is positive int
	then $a ≡ b\;(mod\;m)$ if and only if $(a\;mod\;m) = (b\;mod\;m)$.
<!--ID: 1708098041380-->


### Theorem 3
- a and b are congruent modulo int m <=> there is int k, that $a = b\;+\;km$
<!--ID: 1708098041383-->


### Theorem 4: the congruent modulo of 2 products & sums
- if $a ≡ b (mod\;m)$, and $c ≡ d (mod\;m)$, then
	$a\;+\;c\;≡\;b\;+\;d\;(mod\;m)$
	$ac\;≡\;bd\;(mod\;m)$
<!--ID: 1708098041386-->


### Corollary 5
- m is positive int, a and b are int
	$(a+b) \mod m = ((a \mod m) + (b \mod m)) \mod m$
	$ab \mod m = ((a \mod m)(b \mod m)) \mod m$
	$a^n \mod m = (a \mod m)^n \mod m$
- hard parts:
	- -1 (mod 10) = 9, means adding 9 more to its positive get 10
- how to imagine modulo of negative numbers
	- imagine number line contains only from 0 to 9, and loop back. After 9, we go back to 0. If we start at 0 and move 1 step left (which is -1), we would land on 9
	  => $-1 mod 10 = 9$
<!--ID: 1708098041388-->

### Note on modular arithmetic
- a set $\mathbb{Z}_m$ with both mod addition or multiplication is commutative ring
<!--ID: 1708098041393-->

## addition and multiplication modulo m
- [[Addition modulo operation]]
- [[Multiplication modulo]]
<!--ID: 1708098041397-->

## Application:
- 1. [[Hashing]]
<!--ID: 1708098041402-->
