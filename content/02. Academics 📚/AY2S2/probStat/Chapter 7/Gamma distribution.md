---
mindmap-plugin: basic
tags:
  - Math/statistic/distribution
---

# Gamma distribution

### Description: $X\sim Gamma(\alpha,\lambda)$
- [[Continuous random variable]]
- For $a>0$ and $\lambda >0$
- The gamma distribution with $λ = \frac{1}{2}$ and α = n/2 is called the $χ^2_n$ distribution ([[Chi-squared distribution]]) with n degrees of freedom
- $X\sim Gamma(n,\lambda)$ [[Gamma distribution]] denotes the amount of time one has to wait until a total of $n$ events has occurred knowing avgly $\lambda$ events occurs
- $\lambda$ is the frequency of events happening, how many events per time frame
- Nb of events happened $\sim Po(\lambda t)$
- $X\sim Gam(1,\lambda)=X\sim Exp(\lambda)\to$When $n=1$, its the same as [[Exponential distribution]]
<!--ID: 1708098044218-->


### Probability density function:
- $$f(x)= \frac{\lambda e^{-\lambda x}(\lambda x)^{\alpha-1} }{\Gamma (\alpha)}\text{for } x\ge 0\ \ \ \ \ \ \ \text{and}\ \ \ \ \ \   0 \ \text{for } x<0$$
- Where $\Gamma(\alpha)$ is [[#Gamma function]]
<!--ID: 1708099388656-->


## Gamma function:
- Defined as:$$\Gamma(\alpha)=\int^{\infty}_{0}{\color{tomato}e^{-y}y^{\alpha-1}}dy$$
	- When $\alpha=n\in \mathbb Z^+$:$\Gamma(n)=\color{tomato}(n-1)!$
<!--ID: 1708098044222-->


## Expected value $E[X]=\frac{\alpha}{\lambda}$

## Variance $Var(X)=\frac{\alpha}{\lambda^{2}}$

## Sum of independent Gamma variables:
- If $X\sim Gam(s,\lambda)$ and $Y\sim Gam(t,\lambda)$, then $X+Y\sim ({\color{tomato}s+t},\lambda)$
<!--ID: 1708098044225-->
