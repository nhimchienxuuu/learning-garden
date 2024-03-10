---
tags:
  - Math/statistic
---
# Sum of independent variables
### Description:
- Sum of multiple [[Independent random variable]], then they are [[Jointly distributed random variable]]
- Suppose that $X$ and $Y$ are independent, continuous random variables having PDF $f_X$ and $f_{Y}$. 
- Then the CDF of $\color{tomato}X+Y$ is: $\displaystyle F_{X+Y}=P(X+Y<a)=\int^{\infty}_{-\infty}\int^{a-y}_{-\infty} f_{X}(x).f_{Y}(y)\ dxdy=\begin{cases}\color{tomato}\int^{\infty}_{-\infty} F_X(a-y)f_{Y}(y)\ dy\\ \color{tomato}\int^{\infty}_{-\infty} F_Y(a-x)f_{X}(x)\ dx\end{cases}$
	- Also called the ==convolution== of the distributions $F_X$ and $F_{Y}$
	- $\displaystyle f_{X+Y}={\color{tomato}\int^{\infty}_{-\infty} f_X(a-y)f_{Y}(y)dy}={\color{tomato}\int^{\infty}_{-\infty} f_Y(a-x)f_{X}(x)dx}$
