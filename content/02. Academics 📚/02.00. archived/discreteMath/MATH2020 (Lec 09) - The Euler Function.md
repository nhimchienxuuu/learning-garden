---

mindmap-plugin: basic

---
# The Euler $\phi$ Function
## Euler $\phi$ Function
### Def 1
- Given a positive integer n ∈ N+, define φ(n) to be the number of integers x ∈ N+, x ≤ n such that gcd(x,n) = 1, i.e., the number of integers that are relatively prime with n.
	- example: **When n=5**: The integers from 1 to 5 are 1, 2, 3, 4, and 5. All of 1, 2, 3, and 4 are relatively prime to 5, so ϕ(5)=4.
- <u>in simple terms</u>:
	- relative prime / mutually prime / coprime: when the 2 numbers has $gcd(a,b) = 1$
	- Euler's function: for a given positive int $n$, Euler's function counts how many numbers from 1 to $n$ are relatively prime to $n$
<!--ID: 1708098042045-->

### Theorem 2
- If the prime factorization of n is $n = p_1^{k_1}p_2^{k_2}\cdots p_m^{k_m}$
- $\phi(n) = n\prod_{i} \left(1 - \frac{1}{p_i}\right) = \prod_{i} \left(p_i^{k_i} - p_i^{k_i-1}\right)$
<!--ID: 1708099388769-->


### Corollary 3
$$
\text{If } p \text{ is a prime, then } \phi(p) = p - 1.
$$
- for a prime number p, all numbers **less than p** are relatively prime to p
$$
\text{If } n = pq \text{ where } p \neq q \text{ are both primes, then } \phi(n) = (p - 1)(q - 1).
$$
<!--ID: 1708098042050-->

### Theorem 4 (Euler's Theorem)
- Given $a, n \in \mathbb{N}^+$, if a and n are relatively prime, then: $a^{\phi(n)} \equiv 1 (mod\;n)$
<!--ID: 1708098042055-->


### Corollary 5 (Fermat's Little Theorem)
- If $p$ is a prime and $gcd(a,p) = 1$, then $a^{p-1} \equiv 1 (mod\;p)$
- If $p$ is a prime, for all $a$, $a^p \equiv a(mod\;p)$
<!--ID: 1708098042060-->


### Corollary 6 & 7
- If $gcd(a, n) = 1$, then $a^{\phi(n)−1}$ is an inverse of $a\;mod\;n$
- If $gcd(a, n) = 1$, then $a^x\;\equiv\;a^{x\;mod\;\phi(n)}(mod\;n)$ is an inverse of $a\;mod\;n$
<!--ID: 1708098042064-->


## Euler's Theorem
### Definition 8
- Let $\mathbb{Z}_n^* = \{k | 1 \leq k \in \mathbb{N}^+, k \leq n, \gcd(k, n) = 1\}$
- Consequently: $\phi(n) = |\mathbb{Z}_n^*|$
<!--ID: 1708098042069-->


### Lemma 9
$\text{If } j,k \in \mathbb{Z}_n^*, \text{ then } j \cdot_{n} k \in \mathbb{Z}_n^*.$
<!--ID: 1708098042072-->


### Def 10:
For any element k and subset S of $\mathbb{Z}_n$, let define: $kS \triangleq \{k \cdot_n s | s \in S\}$
<!--ID: 1708098042076-->


### Lemma 11
$\text{If } k \in \mathbb{Z}_n^*, \text{ then } \mathbb{Z}_n^* = k\mathbb{Z}_n^*.$
<!--ID: 1708098042080-->


### Theorem 4 (Euler's Theorem)
$\text{Given } k,n \in \mathbb{N}^+, \text{ if } \gcd(k,n) = 1, \text{ then } k^{\phi(n)} \equiv 1 (\mod n)$
<!--ID: 1708099388770-->


### Primality Test
- <u>Step 1:</u> pick random $a$, such that $1 < a < n$, check if $gcd(a,n) = 1$ and $a^{n-1} \equiv 1\mod{n}$ or not
	- No -> composite number for sure
	- Yes -> probably a prime, continue with different values of $a$
- <u>Step 2:</u> compute $a^k mod n$ efficiently for large $a, n$
	- $ExpMod(a,k,n) = ExpMod(a, k div 2, n)^2 \cdot a ^{k\mod 2}\mod n$
<!--ID: 1708098042086-->


### Chinese Remainder Theorem
- $m_1, m_2, \cdots, m_n$ is pairwise relatively prime positive int > 1
- $a_1, a_2, \cdots, a_n$ arbitrary integers
- Then the system $x \equiv a_1 \pmod{m_1}, x \equiv a_2 \pmod{m_2}, \ldots , x \equiv a_n \pmod{m_n}$
- has a unique solution modulo $m = m_1 m_2 \cdots m_n$ (there is a solution x with $0 \leq x < m$, and all other solutions are congruent modulo m to this solution)
- example
	- Let’s take three moduli m1​=3, m2​=4, and m3​=5 that are pairwise relatively prime (i.e., they don’t share any common factor other than 1).
	- Let’s also take three integers a1​=2, a2​=3, and a3​=1.
	- Now, we have the system of congruences:
	    - x≡2(mod3)
	    - x≡3(mod4)
	    - x≡1(mod5)
	- According to the Chinese Remainder Theorem, this system has a unique solution modulo m=m1​m2​m3​=3∗4∗5=60.
	
	To find the solution, we can use the constructive proof of the Chinese Remainder Theorem:
	
	1. Compute M=m1​m2​m3​=60.
	2. For each i, compute Mi​=M/mi​=60/mi​ and yi​ such that Mi​yi​≡1(modmi​).
	3. The solution is x=(a1​M1​y1​+a2​M2​y2​+a3​M3​y3​)modM.
	
	If you do the calculations, you’ll find that the solution is x=23. This means that 23 is the only number between 0 and 59 that gives a remainder of 2 when divided by 3, a remainder of 3 when divided by 4, and a remainder of 1 when divided by 5.
	
	I hope this example helps illustrate the Chinese Remainder Theorem! Let me know if you have any other questions.
<!--ID: 1708098042093-->

