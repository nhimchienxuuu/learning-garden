---
mindmap-plugin: basic
tags:
  - Math/statistic
aliases:
  - JPDF
---
# Joint probability density function
### Description:
- [[Probability density function|PDF]] for [[Jointly distributed random variable]]
- $X$ and $Y$ are jointly continous for all Continuous random variables, having the property that for every set $C$ of pairs, if there exists a joint probability density function $f(x,y)$ that $P\{(X,Y)\in C\}=\int\int_{(x,y\in C)} f(x,y)\ dx\ dy$
	- Where $f(x,y)$ is the probability of selecting both of them
	- Defining $C=\{(x,y): x\in A, y\in B\}$
	- Then $P\{ X\in A, Y\in B\}=\int_{B}\int_{A}f(x,y)\ dx\ dy$
	- Equivalently $F(a,b)=P\{ X\in (-\infty,a], Y\in (-\infty,b]\}=\int^{b}_{-\infty}\int^{a}_{-\infty}f(x,y)\ dxdy$
	- $f(a,b)=\frac{\partial^2}{\partial a\partial b}F(a,b)$
- If $X$ and $Y$ are jointly continuous, they are individually continuous, and their [[Probability density function|PDF]] is:
	- $\displaystyle\color{tomato}f_{X}(x)=\int^{\infty}_{-\infty}f(x,y)dy$
		- therefore. expectation of 1 variable is $\displaystyle E[X]=\int f_{X}(x)dx=\int\int^{\infty}_{-\infty}x.f(x,y)dydx$
	- $\displaystyle\color{tomato}f_{Y}(y)=\int^{\infty}_{-\infty}f(x,y)dx$
- $\displaystyle P(X\in A)=P\{X\in A, Y\in (-\infty,\infty) \}= \int_A\int^{\infty}_{-\infty} f(x,y)dydx={\color{tomato}\int_{A}f_X(x)dx}$
	- [[Multiple integral#Double integrals over general regions]]

### For number of jointly random variable, $n>2$
- We can also define joint probability distributions for $n$ random variables in exactly the same manner as we did for $n=2$
<!--ID: 1708098044106-->

### Independent random variables
- If the random variable $X$ and $Y$ for any two sets of real numbers $A$ and $B$ $P\{ X\in A, Y\in B\}=P\{X\in A\}. P\{Y\in B\}$
	- $P\{X\le A, Y\le B\}=P\{X\le a\}.P\{Y\le b\}$
	- ${\color{tomato}F(a,b)=F_{X}(a).F_{Y}(b)}\ \ \ \ \text{for all }a,b$
- 2 continuous random variables are independent if and only if their JPDF can be expressed as: $f_{X,Y}=h(x).g(y) \ \ \ \ -\infty<x,y<\infty$
<!--ID: 1708098044110-->

### Expectation of function of joint continuous variable:
- If $X$ and $Y$ have a [[Joint probability density function]] $f (x, y)$, then $\displaystyle E[g(X, Y )] = \int^\infty_{-\infty}\int^\infty_{-\infty}\color{tomato}g(x, y)f (x, y)\ dxdy$
<!--ID: 1708098044113-->
