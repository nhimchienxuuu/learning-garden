---
tags:
  - Math/statistic
---
# Joint distribution of functions of variables
### Description:
- Joint variables but only for continuous's [[Distribution of a function of a random variable]]
- Let $X_1$ and $X_2$ be jointly continuous random variables with [[Joint probability density function]] $f_{X_1, X_2}$.
- Suppose: $Y_1 = g_1(X_1, X_2),\ \  Y_2 = g_2(X_1, X_2)$ for some functions $g_1$ and $g_2$ satisfying:  
	1. The equations $y_1 = g_1(x_1, x_2)$ and $y_2 = g_2(x_1, x_2)$ can be uniquely solved for $x_1$ and $x_2$ in terms of $y_1$ and $y_2$
	2. $g_1$ and $g_2$ have continuous [[Partial derivative#Partial derivatives|partial derivatives]] at all $(x_1, x_2)$ and are such that the [[Jacobian determinant]] $\displaystyle \color{tomato} J(x_1,x_2)\not = 0$
		- Take the absolute of jacobian
 - Then $Y_1$ and $Y_2$ are jointly continous with [[Joint probability density function|JPDF]], $\displaystyle \color{tomato}f_{Y_1Y_2} (y_1, y_2) = f_{X_1,X_2} (x_1, x_2)|J(x_1, x_2)|^{−1}$
	- Replace $x_1,x_2$ with $y_1,y_2$
- For $n>2$:
	- $Y_1=g_1(X_1,...,X_n),...,Y_n=g_n(X_1,...,X_n)$
	- Conditions:
		- $g_i$ all have continuous [[Partial derivative|partial derivative]] and have unique solutions for $x_i$
		- [[Jacobian determinant]], $J(x_1,..,x_n)\not = 0$
		- Then $f_{Y_1,...,Y_n}=f_{X_1,...,X_2}(x_1,...,x_n)|J(x_1,...,x_n)|^{-1}$