---
mindmap-plugin: basic
tags:
  - Math/statistic
---
# Correlation, $\rho$

## Definition
- Correlation refers to any of a broad class of statistical relationship involving dependence
	- dependence is any statistical relationship between 2 random variables or 2 sets of data
	- a typical way of showing the correlation between 2 related variables - [scatter diagram](https://i.imgur.com/Pt9pEHx.png)
	- 
## iow
- **Correlation**: 
	- This is a statistical measure that indicates the extent to which two or more variables fluctuate together
	- A positive correlation indicates the extent to which those variables increase or decrease in parallel; a negative correlation indicates the extent to which one variable increases as the other decreases
	- For example, let’s consider the relationship between the amount of time spent studying and the grades obtained. These two variables are likely to be positively correlated because as the amount of time spent studying increases, the grades obtained also tend to increase.
## Description:
- The correlation of two random variables $X$ and $Y$, denoted by $\rho (X , Y )$
	- defined as long as $Var(X).Var(Y)$ is positive
	- Denotes the degree of linearity:
		- Near +1 or -1 denotes there is a high degree of linearity
		- Near 0 indicates such linearity is absent
## Calculation:
- $\displaystyle\rho(X,Y)=\color{tomato}\frac{\text{Cov}(X,Y)}{\sqrt{Var(X)Var(Y)}}$
	- $-1\le \rho(X,Y)\le 1$
- $\rho(X,Y)=1$ implies $m=\sigma_y/\sigma_x>0$ for $y=mx+c$
- $\rho(X,Y)=-1$ implies $m=-\sigma_y/\sigma_x<0$ for $y=mx+c$

## Degree of correlation
- 2 variables can be
	- [perfectly correlated](https://i.imgur.com/vweRweW.png)
	- [partly correlated](https://i.imgur.com/rUcZnhC.png)
	- [uncorrelated](https://i.imgur.com/MiapxuK.png)

## Correlation coefficient
- The correlation coefficient is $r$
	- measuring the degree of correlation between two variables 
	- ![](https://i.imgur.com/R0qmWHr.png)
	- to **predict** the values for one variable y given the other variable x -> find [[Linear regression#Finding line of best fit|line of best fit]]

## Coefficient of determination:
- $\\(r^2\\)$
	- coef of determination = sqr of correlation coef
	- measures the explanatory power of the regression model; iow, **how well our data fits the regression model** 
	- ranges from 0 to 1
		- 0: none of the variability of the response data around its mean
		- 1: model explains all the variability of the response data around its mean
	- eg: $\\(r^2 = 0.85\\)$ -> 85% of the variation in the dependent variable is explained by the independent variables in the model. the remaining 15% is not explained by the model

## Spearman's rank correlation coefficient
- Spearman's rank correlation coefficient: $R$
	- ![](https://i.imgur.com/MS3ooRl.png)
