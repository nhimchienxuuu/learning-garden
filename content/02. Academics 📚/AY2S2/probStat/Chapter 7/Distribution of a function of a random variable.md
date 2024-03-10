---
mindmap-plugin: basic
tags:
  - Math/statistic
---
# Distribution of a function of a random variable
### Description:
- Let $X$ be a [[Continuous random variable]] having PDF $f_X$. 
- Suppose that $g (x)$ is a strictly ==monotonic==, differentiable function of $x$.
- The random variable $Y$ defined by $Y = g (X )$ has a PDF given by:
	- $f_Y=\begin{cases} f_{X}[g^{-1}(y)] & \bigg| \frac{d}{dy}g^{-1}(y) \bigg| & \text{if } y=g(x)\text{ for some } x\\ 0 &  & \text{if }y\not= g(x) \text{ for all } x \end{cases}$
		- meaning $f_Y=f_{X}[g^{-1}(y)]\times \frac {d}{dy}g^{-1}y$ 
		- Example: 
			- $Y=X^{3}\to P(Y<y)=P(X^{3}<y)=\color{tomato}P(X<\sqrt[3]{y})=F_X(\sqrt[3]y)$ 
			- Differentiate that, we have PDF of $f_X$ in terms of $y$
	- where $g^{-1}(y)$ is defined to be equal to that value of $x$ such that $g(x)=y$