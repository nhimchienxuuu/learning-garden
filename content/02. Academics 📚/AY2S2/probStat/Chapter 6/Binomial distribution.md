---
tags:
  - Math/statistic/distribution
aliases:
  - binomial distribution
---
# Binomial distribution
### Definition: $X\sim B(n, p)$
- When event $X$ has binary response, either fail or success
	- [[Discrete random variable]]
- Condition:
	- The same experiment is repeated a fixed number of times
	- There are only 2 possible outcomes, success and failure
	- The repeated trials are independent, so that the probability of success remains the same for each trial
<!--ID: 1708098043934-->

### Probability mass function
- $P(X=x)\displaystyle=\bigg(\begin{matrix} n\\ x \end{matrix}\bigg)p^xq^{n-x}$
<!--ID: 1708098043939-->

### Expected value $E[X]=np$
- Proof: ^72433b
	- Let $X$ be a binomial random variable with parameters $n$ and $p$
	- Then $X=\sum\limits_{i=1}^nX_i$ where $X_i \begin{cases} 1 & \text{if the ith trial success}\\ 0 & \text{otherwise} \end{cases}$
	- $X_i\sim B(1,p)\to E[X_i]=1*p+0*(1-p)=p$
	- $E[X]=\sum E[X_i] = np$
<!--ID: 1708098043943-->

### Variance $Var(X)=npq$
- Proof:
	- Similarly for [[Binomial distribution#^72433b|above]], $Var(X_i)=p-p^2$
	- $Var(X)=Var(X_1)+...+Var(X_n)=n(p-p^2)=n.p.(1-p)$
<!--ID: 1708098043947-->

### Sum of independent Binomial distribution:
- [[Sum of independent variables]]
- $X\sim B(n,p)$ and $Y\sim B(m,p)$ then $X+Y\sim B(n+m,p)$
<!--ID: 1708098043950-->
