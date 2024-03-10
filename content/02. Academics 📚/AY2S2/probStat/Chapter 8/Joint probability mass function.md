---
mindmap-plugin: basic
tags:
  - Math/statistic
---
# Joint probability mass function
### Description:
- [[Jointly distributed random variable]] for [[Probability mass function]]
- When $X$ and $Y$ are Discrete random variables, define the joint probability mass function of $X$ and $Y$ by $p(x, y ) = P(X = x, Y = y )$
	- $p_X(x)=\sum\limits_{j}p(x,j)$
	- $p_Y(x)=\sum\limits_{i}p(x_i,y)$
### Independent random variables
- If the random variable $X$ and $Y$ for any two sets of real numbers $A$ and $B$ $$P\{ X\in A, Y\in B\}=P\{X\in A\}. P\{Y\in B\}$$
	- For discrete, $p(x,y)=p_{X}(x).p_{Y}(y)\text{ for all }x,y$
	- $P\{X\le A, Y\le B\}=P\{X\le a\}.P\{Y\le b\}$
	- ${\color{tomato}F(a,b)=F_{X}(a).F_{Y}(b)}\ \ \ \ \text{for all }a,b$
- Two discrete random variables are independent if and only if their JPMF can be expressed as: $f_{X,Y}=h(x).g(y) \ \ \ \ -\infty<x,y<\infty$
<!--ID: 1708099388662-->

### Expectation of function of joint discrete variable:
- If $X$ and $Y$ have a [[Joint probability mass function]] $p(x,y)$, then $\displaystyle E[g(X, Y )] =\sum\limits_y \sum\limits_x\color{tomato}g(x,y)f(x,y)$ 
<!--ID: 1708098044127-->
