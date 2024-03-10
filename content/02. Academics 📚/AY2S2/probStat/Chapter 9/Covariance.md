---
mindmap-plugin: basic
tags:
  - Math/statistic
---
# Covariance
### Description:
- To find the "correlation" between 2 variables, and [[Correlation]] is the standard value to easier understood
- If $X$ and $Y$ are independent, then their covariance, $\text{Cov}(X,Y)=0$
- But $\text{Cov}(X,Y)=0$ doesn't mean that they are independent
- ${\color{tomato}\text{Cov}(X,Y)=E[(X-E[X])(Y-E[Y])]=E[XY]-E[X]E[Y]}$
	- [[Expected value]]
### Propositions:
- $\text{Cov}(X,Y)=\text{Cov}(Y,X)$
- $\text{Cov}(X,X)=Var(X)$
	- [[Variance]]
- $\text{Cov}(aX,Y)=a\text{Cov}(X,Y)$
- $\text{Cov}(-X,Y)=-\text{Cov}(X,Y)$
- $\displaystyle\text{Cov}\bigg(\sum\limits^n_{i=1}X_i,\sum\limits^m_{j=1}Y_j\bigg)=\color{tomato}\sum\limits^n_{i=1}\sum\limits^m_{j=1}\text{Cov}(X_i,Y_j)$
- If $Y_j=X_j, j=1,...,n$ 
	- $\displaystyle Var\bigg(\sum\limits^n_{i=1} X_i\bigg)\color{tomato}=\sum\limits^n_{i=1}Var(X_i)+\sum\limits_{i\not= j}\text{Cov}(X_i, X_j)$
	  $\displaystyle=\sum\limits^n_{i=1}Var(X_i)+2\sum\limits_{i<j}\text{Cov}(X_i,X_j)$
	- If $X_i,...,X_n$ are pairwise independent, then $\displaystyle\color{tomato} Var\bigg(\sum\limits^n_{i=1} X_i\bigg)=\sum\limits^n_{i=1}Var(X_i)$
<!--ID: 1708099388628-->

