---
tags:
  - Math/statistic
---
# Markov's inequality
- If $X$ is random variable that takes only non-negative values then for any value $a>0$, then $\color{tomato}\displaystyle \displaystyle P(X\ge a)\le \frac{E[X]}{a}$
- Proof:
	- Let $I$ be indicator variable for $X\ge a$
	- $P(X\ge a)=E[I]$
	- As $X\ge a$ when $I=1$ and $X\ge 0$ when $I=0\to I\le \frac X a\to E[I]\le E[\frac X a]$
	- $P(X\ge a)\le \frac{E[X]}{a}$
---
<!--ID: 1708098043460-->
