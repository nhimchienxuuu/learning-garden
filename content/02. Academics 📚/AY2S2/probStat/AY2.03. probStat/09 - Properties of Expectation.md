---
mindmap-plugin: basic
tags: 
create-time: 05 12 2023 - 00:49
---
# Properties of Expectation
- Proposition:
If $P(a\leq X\leq b)=1$ then $a\le\ E X\le\ b$
<!--ID: 1708098043626-->


## Expectation of Sums of RV
- X and Y have **joint probability mass function (discrete RV)** p(x,y)
	- $E[g(X,Y)]=\sum_{y}\sum_{x}g(x,y)p(x,y)$
- X and Y have **joint probability density function (continuous RV)** f(x,y)
	- $E[g(X,Y)]=\int_{-\infty}^{\infty}\int_{-\infty}^{\infty}g(x,y)f(x,y)\,d x\,d y$
- BSKT:
	- cdf: cumulative distribution function: probability that a random variable (continuous or discrete) take on value $\leq$ certain value
- $X \geq Y$ for random var X and Y => $E[X-Y]\geq0$ => $E X\geq E Y$
- If $E[X_i]$ is finite for all $i = 1,\cdots, n$ => $E[X_{1}+\cdots+X_{n}]=E[X_{1}]+\cdots+E[X_{n}]$
  (expectation of all $X_i$ is sum of expectation of each $X_i$)
- **The sample mean**: 
	- $X_i, \cdots, X_n$ is sequence of independent + identically distributed RV
	- distribution function F, expected value $\mu$
	- sample mean: ${\bar{X}}=\sum_{i=1}^{n}{\frac{X_{i}}{n}}$
	- Expectation: $E\bar{X}=\mu$
- **Expectation of a binomial random variable**
	- X is binomial random variable, parameters $n$ and $p$
	- $X = X_1 + \cdots + X_n$, where $X_{i}=\left\{\begin{array}{l l}{{1}}&{{\mathrm{if~the~ith~trial~is~a~success}}}\\ {{0}}&{{\mathrm{otherwise}}}\end{array}\right.$
	- $X_i$ is Bernoulli RV (see [[06 - Discrete Random Variables#^4a451b| Bernoulli from lec 06]]), with $E[X_i] = p$ => $E[X]=E[X_{1}]+\cdot\cdot\cdot+E[X_{n}]=n p$
<!--ID: 1708098043629-->

## Covariance, Variance of Sums, and Correlations
- BSKT: Expectation calculation
	- DRV: $E[X] = \sum_{}^{}xp(x)$
	- CRV: $E[X] = \int_{-\infty}^{\infty} x\cdot f(x) \,dx$
- X and Y independent -> just like product rule, for functions h and g
	- $E[g(X)h(Y)]=E[g(X)].E[h(Y)]$
- Covariance: give info on relationship btw random vars
	- $Cov(X,Y)=E[(X-E[X])(Y-E[Y])]=E[X Y]-E[X]E[Y]$
	- If X and Y independent => $Cov(X,Y)=0$; the converse is not true
- Covariance proposition:
	- $\mathrm{Cov}(X,Y)=C o v(Y,X)$ -> cov is equal to itself
	- $\mathrm{Cov}(X,Y)=\mathrm{Var}(X)$ -> cov is equal to var of x
	- $\mathrm{Cov}\bigl(\sum_{i=1}^{n}X_{i},\sum_{j=1}^{m}Y_{j}\bigr)=\sum_{i=1}^{n}\sum_{j=1}^{m}\mathrm{Cov}(X_{i},Y)$ -> cov of sum = sum of cov
- If $Y_j = X_j, j = 1,...,n$
	- $\mathrm{Var}\left(\sum_{i=1}^{n}\ X_{i}\right)=\sum_{i=1}^{n}\mathrm{Var}\left(X_{i}\right)+2\sum_{}\sum_{i<j}\mathrm{Cov}(X_{i},X_{j})$
- If $X_1, \cdots, X_n$ are pairwise independent ($X_i$ and $X_j$ independent for $i \neq j$)
	- $Var(\sum_{i=1}^{n}X_i) = \sum_{i=1}^{n}Var(X_i)$ -> var of sum = sum of var
- **Sample variance, variance of sample mean, expectation of sample variance**
	- $X_i, \cdots, X_n$ is sequence of independent + identically distributed RV, expected value $\mu$, variance $\sigma^2$, sample mean $\bar{X}$ 
	  => $S^{2}=\sum_{i=1}^{n}\frac{(X_{i}-{\bar{X}})^{2}}{n-1}$ 
- **Variance of Binomial RV**, para n and p
	- $X = X_1 + \cdots + X_n$, where $X_i$ are independent Bernoulli RV, such that $X_{i}=\left\{\begin{array}{l l}{{1}}&{{\mathrm{if~the~ith~trial~is~a~success}}}\\ {{0}}&{{\mathrm{otherwise}}}\end{array}\right.$
	  => $\operatorname{Var}(X)=\operatorname{Var}(X_{1})+\cdot\cdot\cdot+\operatorname{Var}(X_{n})=n p(1-p)$ as $Var(X_i) = p - p^2$ for all $i$ 
- **Correlation of 2 RV**, $\rho(X,Y)$: 
  => $\rho(X,Y)=\frac{\mathrm{Cov}(X,Y)}{\sqrt{Var(X)Var(Y)}}$
  => $-1\leq\rho(X,Y)\leq1$
  - $\rho(X,Y)=1\mathrm{~implies~}Y=a+b X,\,\mathrm{where~}b=\sigma_{y}/\sigma_{x}>0$
  - $\rho(X,Y)=-1\mathrm{~implies~}Y=a+b X,\,b=-\sigma_{y}/\sigma_{x}<0$
  - Correlation coefficient: measure of degree of linearity btw X, Y
	  - $\rho(X,Y)\;near\;1$ or $\rho(X,Y)\;near\;-1$ => high linearity btw X and Y
	  - $\rho(X,Y)\;near\;0$ => absent linearity
	  - $\rho(X,Y) = 0$ => uncorrelated
	  - $\rho(X,Y) > 0$: Y increases when X increases
	  - $\rho(X,Y)<0$: Y decreases when X increases
- **Conditional Expectation**
	- DRV: $E[X|Y=y]=\sum_{x}x P(X=x|Y=y)$, for all y such that $p_{Y}(y)>0$
	- CRV: $E[X|Y=y]=\int_{-\infty}^{\infty}x f_{X\mid Y}(x|y)d x$, where $f_{X|Y}(x|y)={\frac{f(x,y)}{f_{Y}(y)}}$
	- BSKT: 
		- $f_{X}(x)=\int_{-\infty}^{\infty}f(x,y)\,d y$ -> integrate w.r.t $y$
		- $f_{Y}(y)=\int_{-\infty}^{\infty}\mathcal{f}(x,y)\,d x$ -> integrate w.r.t $x$
	- Conditional expectation satisfy properties of ordinary expectation
		- $E[g(X)|Y=y]={\left\{\begin{array}{l l}{\displaystyle\sum_{x}g(x)p_{X|Y}(x|y){\mathrm{~in~the~discrete~case}}}\\ {\displaystyle\int_{-\infty}^{\infty}g(x)f_{X|Y}(x|y)\,d x}\;{\mathrm{~in~the~continuous~case}}\end{array}\right.}$
		- $E\left[\sum_{i=1}^{n}X_{i}|Y=y\right]=\sum_{i=1}^{n}E[X_{i}|Y=y]$
	- Computing Expectations by Conditioning
		- $E[X]=E[E[X|Y]]$
		- If Y is DRV: $E[X]=\sum_{y}E[X|Y=y]P\{Y=y\}$
		- If Y is CRV, density $f_{Y}(y)$: $E[X]=\int_{-\infty}^{\infty}E[X|Y=y]f_{Y}(y)\,d y$
- **Computing Probabilities by Conditioning**
	- A: arbitrary event; Indicator random variable X by
	  $X={\left\{\begin{array}{l l}{1}&{{\mathrm{if~A~occurs}}}\\ {0}&{{\mathrm{if~A~does~not~occur}}}\end{array}\right.}$
	  => $E[X]=P(A)$
	  => $E[X]Y=y]=P(A|Y=y)$, for RV Y
	- DRV Y: $P(A)=\sum_{y}P(A|Y=y)P(Y=y)$
	- CRV Y: $P(A)=\int_{-\infty}^{\infty}P(A|Y=y)f_{Y}(y)\,d y$
- Conditional Variance:
	- $\operatorname{Var}(X|Y)=E[(X-E[X|Y])^{2}|Y]=E[X^{2}|Y]-(E[X|Y])^{2}$
	- $E[Var(X|Y)]=E[X^{2}]-E[(E[X|Y])^{2}]$
	- $\textstyle\operatorname{Var}(E[X\vert Y])=E[(E[X\vert Y])^{2}]-(E[X])^{2}$
	- $\operatorname{Var}(X)=E[\operatorname{Var}(X|Y)]+\operatorname{Var}(E[X|Y])$
<!--ID: 1708098043633-->

