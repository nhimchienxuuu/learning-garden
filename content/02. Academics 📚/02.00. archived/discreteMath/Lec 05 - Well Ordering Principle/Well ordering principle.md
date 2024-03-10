---
mindmap-plugin: basic
tags:
  - Math/discrete/principle
---

# Well ordering principle

## WOP 
### WOP Description:
- Every non-empty set of non-negative integers has a smallest element
<!--ID: 1708098041172-->


## Factoring Primes
### Claim 2:
- Any positive integers m and n, the fraction $\frac{m}{n}$ can be written in lowest terms
	- as they are positive int, we can simplify the fraction by dividing with $gcd(m,n)$ -> lowest terms
<!--ID: 1708098041178-->

### Theorem 3:
- Every positive integer greater than 1 can be factored as a product of primes
	- 3 = 3* 1
	- 9 = 3 * 3
	- 10 = 2 * 5
<!--ID: 1708098041181-->

## Round-robin tournament
### Definition
- a competition where each player meets every other players, contrast with elimination (eliminated after certain losses)
- $p_1$ beats $p_2$, ... , $p_n-1$ beats $p_n$, $p_n$ beats $p_1$
- see the directed graph representation [[Pasted image 20231124232143.png|here]],edges go from winner to loser
<!--ID: 1708098041186-->

### Claim 4 ❗️❗️❗️
- If there is cycle length m ($m \geq 3$) among players in round-robin tournament, there must be a cycle of three of these players
	- a cycle is a sequence of players such that $p_1$ beats $p_2$, ... , $p_n$ beats $p_1$
<!--ID: 1708098041191-->



## Well Ordered Sets
### Theorem 5: 
- For any nonnegative int n, the set of integers $\geq -n$ is well ordered
	- consider this is the set S
	- increase each element in the set by n -> not change relative order -> apply the WOP -> there is a smallest element in the set S (denote as m)
	- we get $m-n$ is the actual smallest element of S
<!--ID: 1708098041196-->


### Definition 6
- lower bound of set S is $b \leq s$, for every $s \in S$, $S$ is set of real numbers) -> b is the smallest number in S
- upper bound of set S is $b \geq s$, for every $s \in S$, $S$ is set of real numbers) -> b is the largest number in S
<!--ID: 1708098041201-->


### Corollary 7
- any set of integers with a lower bound is well ordered
<!--ID: 1708098041204-->
