---
mindmap-plugin: basic
tags:
  - Math/statistic
---

# Continuous random variable

### Definition
- If there exists a nonnegative Probability density function $f$, defined for all real $x\in (-\infty ,\infty)$, having the property for any set $B$ of real numbers, $P(X\in B)=\int_{B}f(x)dx$
- $\displaystyle P(a\le X\le b)=\int^b_{a}f(x)$
- $\displaystyle P(X=A)=\int^a_a=0$
	- Hence, $P(X\le a)=P(X\le A)$
### [[Expected value]]:
- $\displaystyle E(X)=\int^{\infty}_{-\infty}x.f(x)dx$
- $\displaystyle E(g(X))=\int^{\infty}_{-\infty}g(x)\ f(x)\ dx$
<!--ID: 1708098044193-->

### [[Variance]]:
- If $X$ is a random variable with expected value, $\mu$
	- $\displaystyle Var(X)=E[(X-\mu)^2]=E[X^2]-(E[X])^{2}=\color{tomato}\int^{\infty}_{-\infty}x^{2}f(x)dx-(E[X])^2dx$
	- $\sigma_X=\sqrt{Var(X)}$
- Related variable:
	- $Var(aX\pm b)=a^2Var(X)$
	- $Var(X\pm Y)=Var(X)+Var(Y)$
<!--ID: 1708098044197-->
