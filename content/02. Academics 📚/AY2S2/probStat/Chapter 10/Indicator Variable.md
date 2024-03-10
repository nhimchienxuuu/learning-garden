---
tags:
  - Math/statistic
---
# Indicator Variable
### Description:
- Let random variable $I$ be indicator variable for event $A$, $I=1$ if $A$ occurs, 0 otherwise
- Then, for any random variable $Y$:
	- $\color{tomato}E[X]=P(A)$
	- $\color{tomato} E[X|Y=y]=P(A|Y=y)$
	- For discrete: $\displaystyle P(A)=\sum\limits_y P(A|Y=y).P(Y=y)$
		- which is Conditional probability
	- For continuous: $P(A)=\displaystyle \color{tomato}\int ^\infty_{-\infty}P(A|Y=y).f_Y(y)dy$
- When $X$ is an indicator variable for $n$ events:
	- $\displaystyle E[X^2]=E[X_1. X_2]= \sum\limits_{i=1}^n \sum\limits_{j=1}^n  E[X_i.X_j]= \sum\limits_{i=1}^n E[X_i^2]+\sum\limits_{i\not= j}^n E[X_i.X_j]$
	   $\displaystyle =E[X]+2\sum\limits_{i< j}^n E[X_i.X_j]$
		- $E[X_i^2]=E[X_i]$
		- 