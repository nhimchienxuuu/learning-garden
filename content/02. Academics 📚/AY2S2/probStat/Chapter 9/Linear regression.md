---
tags:
  - Math/statistic
aliases:
  - Linear prediction
---
# Linear regression
## Description:
- [[Prediction]] by [[Regression Model]]
- We might not know the PDF of $X$ and $Y$, but if we know the mean and standard variance, we can determine the best linear predictor of $Y$ with respect to $X$

## Finding line of best fit
- 2 main methods:
	1. Scattergraph method:
	    - Draw a line through data points with about an equal number of points above and below the line.
	2. Linear regression:
		- Using [[least squares method]]
	    - Using correlation:
	        - We need to choose a and b to minimize the [[Mean square error]]
			- $\\({\color{tomato}E [(Y − (a + bX ))^2]} =E [Y^2] − 2aE [Y ] − 2bE [XY ] + a^2 +2abE [X ] + b^2E [X ^2]\\)$
			- Taking partial derivative and set them equal to 0 we have $a$ and $b$ when it is at minimum point
				- Cant have maximum due to the nature of the problem
			- $\displaystyle b=\frac{\text{Cov}(X,Y)}{\sigma^2_X}$
			- $a=E[Y]-bE[X]$
			- The best linear predictor (lowest mean square error) is: $\mu_y+\frac{\rho\sigma_y}{\sigma_x}(X-\mu_x)$
				- Happens when $\mu_y=E[Y],\mu_y=E[X]$ and $\rho$ is the [[Correlation]] of $X$ and $Y$
				- The [[Mean square error]] of this predictor is given by $\displaystyle E[(Y -\mu_y - \frac{\rho\sigma_y}{\sigma_x}(X - \mu_x )^2]= \sigma^2_y (1 - \rho^2)$
		- Using $\\(y = a + bX\\)$ 
			- $\\({b}=\frac{n\sum x_{i}y_{i}-\sum x_{i}\sum y_{i}}{\sqrt{n\sum x_{i}^{2}-(\sum x_{i})^{2}}}\\)$ 
			- $\\(a={\frac{\sum y}{n}}-{\frac{b\sum x}{n}}\\)$
## Assumptions about error term ϵ in linear regression model:
1. $\\(E(ϵ)=0\\)$. This implies $β_0​$ and $β_1$​ are constants, and hence $\\(E(y)=β0​+β1​x\\)$
2. The variance of ε, denoted by $(\\\sigma^2\\)$, is the same for all x
3. The values of ε are independent.
4. ε is a normally distributed random variable for all values of x

## [[Regression Model#Testing for significance|Testing for significance]]
- If $\\(β_1​=0\\)$, then $(\\E(y)=β_0\\)​$. In this case, we would conclude that x and y are not linearly related
- If $\\(β1\ne0\\)$, we would conclude that the two variables are related.

- Thus, to test for a significant regression relationship, we must **conduct a hypothesis test** to determine whether $\\(β_1​=0\\)$
- The [[Hypothesis Testing#For t-value|t-test]] is commonly used.
	- ![](https://i.imgur.com/sR5YCqd.png)
	- ![](https://i.imgur.com/x0pgOmP.png)
	- ![](https://i.imgur.com/GhTBZRX.png)

