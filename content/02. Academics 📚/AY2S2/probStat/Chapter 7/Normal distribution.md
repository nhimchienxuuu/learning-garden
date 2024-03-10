---
mindmap-plugin: basic
aliases:
  - bell curve
  - normal random variable
  - normally distributed
tags:
  - Math/statistic/distribution
---

# Normal distribution

### Definition: $X\sim N(\mu,\sigma^2)$
- [[Continuous random variable]]
- based on [[Standard normal distribution]]
- We say that $X$ is normal random variable, or simply that $X$ is [[Normal distribution|normally distributed]], with parameters $\mu$ and $\sigma^2$ denoted by $X\sim N(\mu,\sigma^2)$
	- $X\sim N(5,10)$
<!--ID: 1708098044229-->


	-
	  ```functionplot
	  ---
	  xLabel:
	  yLabel:
	  bounds: [-5,15,0,0.15]
	  disableZoom: true
	  grid: true
	  ---
	  f(x)=1/(sqrt(2*PI)*sqrt(10))* E^(-(x-5)^2/(2*10))
	  ```

- Properties:
	- $\int^{\infty}_{-\infty} f(x)dx=1$
	- Expected value $E[X]=\mu$
	- Variance $Var(x)=\sigma^2$
	- Graph of $f$ is symmetric in the line $x=\mu$
	- $f$ is maximized when $x=\mu$
	- $f$ has two [[Infection point]]s at $x=\mu \pm \mu$
- Conditions
	- $f(x)\ge 0 \ \forall x\in (-\infty,\infty)$

### [[Probability density function]]
- $\displaystyle f(x)=\frac{1}{\sqrt{2\pi}\sigma}e^{-\frac{(x-\mu)^2}{2\sigma^{2}}},\infty<x<\infty$
<!--ID: 1708098044233-->


### Normal approximation to [[Binomial distribution]]:
- Use [[The DeMoivre-Laplace limit theorem]] to evaluate a [[Binomial distribution]] when the number of trials become large.
- $X\sim B(n,p)\to X\sim N({\color{red}np,npq})$ where:
	- $np\ge 5$
	- $nq=n(1-p)\ge 5$
- Continuity correction:
	- Convert from discrete integer valued (binomial) to continuous (normal)
	- $P(X = i)$ as $P(i − 0.5 < X < i + 0.5)$
	- $P(X<i)\to P(X<i+0.5)$
	- $P(X\le i)\to P(X<-0.5)$
	- $P(X>i)\to P(X<i+0.5)$
	- $P(X\ge i)\to P(X<i-0.5)$
<!--ID: 1708098044236-->


### Sum of independent normal distribution:
- [[Sum of independent variables]]
- If $X_{i}\sim N(\mu_{i},\sigma^{2}_{i})$, then $\sum\limits_{i=1}^{n}X_{i}\sim N\bigg(\sum\limits_{i=1}^{n}\mu_{i},\sum\limits_{i=1}^{n}\sigma^2_{i}\bigg)$
<!--ID: 1708098044240-->


