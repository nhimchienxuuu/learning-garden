---
tags:
  - Math/discrete/theorem
---
# Chinese remainder theorem
### Description:
- Let $m_{1}, m_{2}, ...,m_{n}$ be pairwise [[Prime number#Relative primality|relatively prime]] positive integers greater than 1 and  $a_{1},a_{2},...,a_{n}$ arbitrary integers. 
	- Then the system$\begin{cases} x\equiv a_{1}\mod m_{1}\\ x\equiv a_{2}\mod m_{2}\\...\\ x\equiv a_{n}\mod m_{n}\end{cases}$ has a unique solution modulo $m=m_{1}m_{2},...,m_{n}$
	- That is, there is a solution $x$ with $0 ≤ x < m$, and all other solutions are congruent modulo $m$ to this solution
### Uniqueness
- Let assume $0 <= x, y < m$ be solution, then $m_k |y − x \text{ for all }  k = 1, 2, . . . , n$ (why?).
- Hence, $m = m_{1}m_{2} · · · m_{n}$ and $m|y − x$
	- note $|y − x| < m$, we must have $y − x = 0$, or $x = y$
<!--ID: 1708098041467-->

### Existence
- Define $M_{k} = m/m_{k}$ for $k = 1, 2, . . . , n$. We can show $gcd(m_k , M_k ) = 1$
- Thus, there exists an integer $y_{k}$ such that $M_{k} y_{k} ≡ 1 \mod m_{k}$ 
	- Find inverse by [[Euler's theorem#^4b2036]]
- We can show $x \equiv a_1M_1y_1 + a_2M_2y_2 + · · · + a_nM_ny_{n}\mod m$ is a solution
<!--ID: 1708098041470-->
