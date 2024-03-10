---
tags:
  - Math/statistic/test
---
TARGET DECK: probStat/chapter12
# Hypothesis Testing
## Description:
- ![](https://sixsigmadsi.com/wp-content/uploads/2021/06/Type-I-and-II-errors.jpg)
## Using [[Confidence interval]]:
- To test claims about a population mean $\mu$, we construct a confidence interval (a, b).
	- Claim: $\mu = \mu_0$ Do not reject test-claim if $\mu_0\in (a, b)$, reject otherwise.
	- Claim: $\mu< \mu_0$. Do not reject test-claim if $b < \mu_0$, reject otherwise.
	- Claim: $\mu>\mu_0$. Do not reject test-claim if $\mu_0<a$ , reject otherwise.

## [[Null Hypothesis]] and [[Alternative Hypothesis]]
## One-tailed vs two-tailed:
1. $H_0:\mu \ge \mu_0, \ H_a:\mu< \mu_0$, lower one-tailed
2. $H_0: \mu \le \mu_0, \ H_a: \mu> \mu_0$, upper one-tailed
3. $H_1: \mu=\mu_0, \ H_a:\mu\not = \mu_0$, two-tailed

## Test statistic:
- Used to compare against another critical value to evaluate hypothesis
- All test statistic value must lie outside of [[Confidence interval]] $1-\alpha$, to be rejected
### For p-value:
- Use [[Normal distribution]], $\displaystyle ts=\frac{\bar x -\mu_0}{\sigma_x}$ 
- for two-tailed, $p$-value is divided by 2
### For t-value:
- Use [[t distribution]], $\displaystyle ts=\frac{\bar x -\mu_0}{s/\sqrt n}$ at $n-1$ def
- then convert to $p$-value (area under graph) at $n-1$ df
### For Proportion:
- Use [[Confidence interval#For population proportional|Population proportion]]
- $$\displaystyle ts=\frac{\bar p - {\color{tomato}p_0}}{\sqrt{\color{tomato}\frac{p_0.(1-p_0)}n}}$$
### For [[Difference random variable of 2 variables]]:
- For known $\sigma$
	- Because $\bar x_1-\bar x_2\sim N(D_0, \sqrt{\frac{\sigma^2_1}{n_1}+\frac{\sigma^2_2}{n_2}})$ 
	- $\displaystyle ts= z=\frac{\bar x_1-\bar x_2 -D_0}{\sqrt{\frac{\sigma^2_1}{n_1}+\frac{\sigma^2_2}{n_2}}}$ 
		- $D_0=\mu_1-\mu_2$
- For unknown $\sigma$
	- Then use t-distribution with degree of freedom
	- $$\displaystyle df=\frac{\bigg(\frac{s^2_1}{n_1}+\frac{s^2_2}{n_2}\bigg)^2}{\frac1{n_1-1}\bigg(\frac{s^2_1}{n_1}\bigg)^2+\frac1{n_2-1}\bigg(\frac{s^2_2}{n_2}\bigg)^2}$$
		- Round **down** for more conservative interval estimation

## [[Type 1 Error]] vs [[Type 2 Error]]
## Level of significance:
- Same as probability of making a [[Type 1 Error]] 
- When the null hypothesis is true as an equality
- If the cost of making a Type I error is high, small values of α are preferred. 
	- Like medication, must have small LoS
- If the cost of making a Type I error is not too high, larger values of α are typically used.
	- it is ok to make mistake
