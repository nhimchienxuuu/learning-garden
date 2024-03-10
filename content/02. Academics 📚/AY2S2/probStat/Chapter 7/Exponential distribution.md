---
mindmap-plugin: basic
tags:
  - Math/statistic/distribution
aliases:
  - Exponential random variable
---

# Exponential distribution

## Description:
- [[Continuous random variable]]
- Describes the time between events that occur randomly and independently at a constant average rate. the number of occurrence in a timeframe is $\lambda$
- It is often used to model waiting times, such as the time it takes for a customer to be served at a checkout counter or the time it takes for a website to load.
### Probability density function:
- For some $\lambda>0$ by $f(x)=\begin{cases} {\color{tomato}\lambda e^{-\lambda x}} &\text{for } x\ge 0 \\ 0 &\text{for } x<0 \end{cases}$
<!--ID: 1708098044202-->


- $X\sim Exp(1/8)$

	-
	  ```functionplot
	  ---
	  xLabel: x
	  yLabel: P(X)
	  bounds: [0, 50, 0, 0.2]
	  disableZoom: true
	  grid: true
	  ---
	  h(x)= (1/8)E^(-x/8)
	  ```

## Expected value $E[X]=\frac{1}{\lambda}$

## Variance $Var(X)=\frac{1}{\lambda^{2}}$
## Cumulative distribution function:
- $$F(a)=P(X\le a)={\color{tomato}1-e^{-\lambda a}}, \ \ a\ge 0$$
<!--ID: 1708098044206-->


## [[Hazard rate function]] 
- Suppose now that the lifetime distribution is ==exponential== ^bf4248
- Then, by the memory-less property, it follows that the distribution of remaining life for a $t-$year-old item is the same as that for a new item.
- Hence, λ(t) should be constant. In fact, this checks out, since $$λ(t) = \frac{f(t)}{\bar F(t)}=\frac{λe^{−λt}}{e^{−λt}} = λ$$ ^ca9e8d
- Thus, the failure rate function for the exponential distribution is ==constant==.
<!--ID: 1708098044211-->
