---
tags: 
aliases: 
mindmap-plugin: basic
---
# Continuous Random Variables
## PD vs CD
- PD: probability density: calculate at specific point $P(X=k)$ -> f(a)
- CD: cumulative distribution: calculate within a range $P(a \leq X \leq b)$ -> F(a)
- pdf = deri cdf
<!--ID: 1708098043564-->


## Definition
- X is a continuous random variable (CRV) if 
	$P(X \in B) = \int_B f(x)dx$ 
	$f$: nonnegative function
	$x \in (-\infty, \infty)$
	$B$ is a set of real numbers
- function $f$, probability density function of the RV $X$, must satisfy $\int_{-\infty}^{\infty} f(x) = 1$
- We have 
	  $P(a \leq X \leq b) = \int_{a}^{b} f(x) \,dx$ 
	  $P(X = a) = \int_{a}^{a} f(x) \,dx = 0$
  Hence $P(X \leq a) = P(X < a)$


## Expected Value
- If X is a CRV having f(x),
	$E[X] = \int_{-\infty}^{\infty} x\cdot f(x) \,dx$
<!--ID: 1708098043576-->


## Proposition
- X a CRV with f(x), for real-valued g
	$E[g(X)] = \int_{-\infty}^{\infty} g(x)\cdot f(x) \,dx$
<!--ID: 1708098043582-->


## Corollary
- a, b const: $E[aX + b] = aE[X] + b$
<!--ID: 1708098043586-->


## Variance & standard deviation
- ![[Pasted image 20231118151736.png]]
<!--ID: 1708098043591-->


## Uniform distribution
- ![[Pasted image 20231118151840.png]]
- Probability of uniform distribution
	$P(x_1 < X < x_2) = \frac{x_2 - x_1}{b - a}$
![[Pasted image 20231119122748.png]]
<!--ID: 1708098043596-->


## Normal distribution
![[Pasted image 20231118151858.png]]
![[Pasted image 20231118151924.png]]
![[Pasted image 20231118152022.png]]
<!--ID: 1708098043603-->


## Standard Normal Distribution
![[Pasted image 20231118152043.png]]
![[Pasted image 20231118152110.png]]![[Pasted image 20231118204717.png]]
- area of z-value is to the left
- determine value of z on z-table: z = 1.56 -> 1.5 in rows - vertical, 0.06 in columns - horizontal
<!--ID: 1708098043607-->


## Normal Approximation to Binomial Distribution
- trials are large, evaluate bino is difficult
	  satisfy $np \geq 5$, $n(1-p) \geq 5$
	normal distribution can be used to approx
<!--ID: 1708098043612-->


- how to use normal approx to bino
	- satisfy $np \geq 5$, $n(1-p) \geq 5$, set $\mu = np, \sigma = \sqrt{np(1-p)}$
	- set $\mu = np, \sigma = \sqrt{np(1-p)}$ in definition of the normal curve
	- Bino is discrete integer-valued RV
	- Normal is continuous RV
	- continuity correction: 
		$P(X = i)$ ->$P(i-0.5 < X < i+0.5)$
		$np \geq 5$, $n(1-p) \geq 5$, set $\mu = np, \sigma = \sqrt{np(1-p)}$

- DeMoivre-Laplace limit theorem
	- normal approx to bino is result of this theorem, which is special case of central limit theorem
## Exponential Random Variables
![[Pasted image 20231118215309.png]]
![[Pasted image 20231118215331.png]]
- Note
	- $X<x$: approx with normal approx bino
	- $X = x$: approx with poisson
<!--ID: 1708098043620-->
