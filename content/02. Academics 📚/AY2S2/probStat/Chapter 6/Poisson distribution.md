---
mindmap-plugin: basic
tags:
  - Math/statistic/distribution
---

# Poisson distribution

### Definition: $X\sim Po(\lambda)$
- [[Discrete random variable]]
- With assumptions:
	- Events occur singly, randomly and independently
	- at consistent rate in a given interval of space/time
- No fixed range of value, extreme values can be happened, but the chance is insignificant
- $\lambda$ is both mean and variance
- Example: number of misprints on a page
<!--ID: 1708098043976-->

### Probability mass function
- $\displaystyle P(X=i)=\color{tomato} e^{-\lambda} \frac{\lambda^i}{i!}$ for $i =0,1,2,...,\infty$
	- $\displaystyle \sum^\infty_{i=0} p(i)=e^{-\lambda}\sum^\infty_{i=0}\frac{\lambda ^i}{i!}=e^{-\lambda}.e^{\lambda}=1$
<!--ID: 1708099388676-->

### Expected value $E[X]=\lambda$
### Variance $Var(X)=\lambda$
### Poisson approximation for [[Binomial distribution|binomial distribution]]:
- Can be used to approximate binomial distribution when:
	- $n$ is large
	- $p$ is small enough so that $\lambda=np$ is of moderate size
<!--ID: 1708098043982-->

### Computing the poisson distribution function:
- $\displaystyle \frac{P(X=i+1)}{P(X=i)}=\frac{\lambda}{i+1}$
<!--ID: 1708098043987-->

### Sum of independent Poisson distribution:
- $X\sim Po(\lambda_{1})$ and $Y\sim Po(\lambda_{2})$, then $X+Y\sim Po(\lambda_{1}+\lambda_{2})$
<!--ID: 1708098043991-->
