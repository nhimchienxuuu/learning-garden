---
tags:
  - Math/statistic
---
# Conditional expectation
### Description:
- [[Conditional joint distribution]] and [[Expected value|Expectation]]
- Discrete case:
	- The conditional expectation of $X$ given $Y=y$, $\color{tomato}\displaystyle E[X|Y=y]=\sum\limits_x xp(X=x|Y=y)$
	- $\displaystyle E[g(X)|Y=y]=\sum\limits_x g(x)p(X=x|Y=y)$
- Continuous case:
	- $\color{tomato}\displaystyle E[X|Y=y]=\int ^{\infty}_{-\infty} x.f_{X|Y}(x|y)dx$
		- where $\displaystyle f_{X|Y}(x|y)=\frac{f(x,y)}{f_Y(y)}$ as in Conditional joint distribution
	- $\displaystyle E[g(X)|Y=y]=\int ^{\infty}_{-\infty} g(x).f_{X|Y}(x|y)dx$
- $\displaystyle E\bigg[ \sum\limits^n_{i=1} [x_i|Y=y]\bigg] = \sum\limits^n_{i=1}E[X_i|Y=y]$
- Think of $E[X|Y]$ is itself a random variable. $\displaystyle E[X]=E[E[X|Y]]$ meaning:
	- For discrete: $E[X]=\color{tomato}\sum\limits_y E[X|Y=y].P(Y=y)$
		- To calculate $E[X]$, we may take a weighted average of the conditional expected value of $X$ given that $Y = y$, each of the terms $E[X|Y = y]$ being weighted by the probability of the event on which it is conditioned.
	- For continuous: $\displaystyle E[X]=\color{tomato}\int^\infty_{-\infty} E[X|Y=y].f_Y(y)dy$
---