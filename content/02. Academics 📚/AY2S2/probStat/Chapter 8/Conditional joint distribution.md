---
tags:
  - Math/statistic
---
# Conditional joint distribution
### Description:
- [[Conditional probability]] and [[Jointly distributed random variable]]
### Discrete case:
- $\displaystyle p_{X|Y}(x|y)=P(X=x|Y=y)=\frac{P(X=x,Y=y)}{P(Y=y)}=\color{tomato}\frac{p(x,{y})}{{p_{Y}(y)}}$
- for all $y$ such that $p_{Y}(y)>0$
	- $F_{X|Y}(x|y)=P(X\le x|Y\le y)=\sum\limits_{a\le x}p_{X|Y}(a|y)$
<!--ID: 1708098044092-->

### Continuous case:
- $\displaystyle{\color{tomato}\displaystyle f_{X|Y} (x|y)}=P(X=x|Y=y)=\frac{P(X=x,Y=y)}{P(Y=y)}={\color{tomato}\frac{f(x,y)}{f_{Y}(y)}}$
	- for all $y$ such that $f_{Y}(y)>0$
- If $X$ and $Y$ are jointly continuous then the [[Joint cumulative distribution function]]:
	- $\displaystyle P(X\in A|Y=y)=\int_{A}f_{X|Y} (x|y)dx$
	- $\displaystyle F_{X|Y}(a|y)=P(X\le a|Y=y)=\int^{a}_{-\infty}f_{X|Y}(x|y)dx$
		- contains $y$ after integration, otherwise independent
---
<!--ID: 1708098044096-->
