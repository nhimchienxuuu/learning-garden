---

mindmap-plugin: basic

---
# Well Ordering Principle
## The Well-ordering Property
### Theorem 1: the WOP
- Every nonempty set of nonnegative integers has a smallest element
	- eg. set of natural numbers N has smallest element of 0
<!--ID: 1708098041756-->


## Factoring Primes
### Claim 2:
- Any positive integers m and n, the fraction $\frac{m}{n}$ can be written in lowest terms
	- as they are positive int, we can simplify the fraction by dividing with $gcd(m,n)$ -> lowest terms
<!--ID: 1708099388787-->

### Theorem 3:
- Every positive integer greater than 1 can be factored as a product of primes
	- 3 = 3* 1
	- 9 = 3 * 3
	- 10 = 2 * 5
<!--ID: 1708099388788-->


### Round-robin tournament
- a competition where each player meets every other players, contrast with elimination (eliminated after certain losses)
- $p_1$ beats $p_2$, ... , $p_n-1$ beats $p_n$, $p_n$ beats $p_1$
- see the directed graph representation [[Pasted image 20231124232143.png|here]],edges go from winner to loser
<!--ID: 1708098041764-->

#### Claim 4 ❗️❗️❗️
- If there is cycle length m ($m \geq 3$) among players in round-robin tournament, there must be a cycle of three of these players
	- a cycle is a sequence of players such that $p_1$ beats $p_2$, ... , $p_n$ beats $p_1$
<!--ID: 1708099388789-->



## Well Ordered Sets
### Theorem 5: 
- For any nonnegative int n, the set of integers $\geq -n$ is well ordered
	- consider this is the set S
	- increase each element in the set by n -> not change relative order -> apply the WOP -> there is a smallest element in the set S (denote as m)
	- we get $m-n$ is the actual smallest element of S
<!--ID: 1708099388790-->


### Definition 6
- lower bound of set S is $b \leq s$, for every $s \in S$, $S$ is set of real numbers) -> b is the smallest number in S
- upper bound of set S is $b \geq s$, for every $s \in S$, $S$ is set of real numbers) -> b is the largest number in S
<!--ID: 1708099388791-->


### Corollary 7
- any set of integers with a lower bound is well ordered
<!--ID: 1708099388792-->



## Infinite Decent Principle
### Definition 8 (Infinite Descent Principle)
- Let P is a property for nonnegative integers
- Assume P(0) is true
- for all $k \in \mathbb{N}$, if $P(k)$ is false, there exist an $m < k$ that $P(m)$ is also false -> contradicting to the WOP
- Then, $P(n)$ is true for all $n \in \mathbb{N}$, including $k$
- <u>Example</u>: 
	- P(n): “n is a positive integer that is not divisible by any square number other than 1”
	- assume there exists a k satisfies P(n)
	- k is not divisible by any square number other than 1. 
	- but every positive number is divisible by 1^2 (which is 1) -> there exists a smaller number m where m = k/ 1^2 = k satisfies P(n). 
	- but this is still k and we are not actually finding a new number, contradicts that we could keep finding a smaller numbers satisfies P, leading to infinite descent
- <u>Core situation:</u> 
	- we can keep finding smaller and smaller natural numbers violating a property >< in a set of natural numbers, there is a smallest element (WOP)
	- if $P(k)$ is true, there will be $P(m)$ and infinite descent numbers of $m$, contradicting with the WOP
<!--ID: 1708098041770-->



### Proposition 1:
- There is no infinite strictly decreasing sequence of natural numbers
<!--ID: 1708098041773-->


## Fermat's Last Theorem for n = 3, 4
### Theorem 9:
- The following equation has no positive integers solution $x^3 + y^3 = z^3$
<!--ID: 1708099388794-->


### Theorem 10:
- The following equation has no positive integers solution $x^4 + y^4 = z^4$
<!--ID: 1708099388795-->

