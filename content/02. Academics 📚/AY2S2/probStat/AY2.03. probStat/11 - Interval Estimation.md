---
mindmap-plugin: basic
time: 
tags: 
source:
---
# 11 - Interval Estimation

### General Info
- sample cannot tell exact population mean $\mu$ -> use sample mean to predict interval of confidence that population mean will lie in -> confidence interval
<!--ID: 1708098043681-->


| note | sample    | population |
| ---- | --------- | ---------- |
| mean | $\bar{x}$ | $\mu$      |
| std     | $s$       | $\sigma$   |

### Normal distribution of Sample mean

- $\bar{X_n}$ normally distributed with mean $\mu$ and std $\sigma / \sqrt{n}$ ([[Practical Interpretation of Limit Theorems]])
	- standard normal random var / test statistic: $Z=\frac{\bar{X_{n}}-\mu}{\sigma/\sqrt{n}}$, $Z\sim N(0,1^{2}).$ *(tag normal random var using z-test)*
	- eg. 95% confidence interval -> find $a$ in $P(-a \leq Z \leq a) = 0.95$ -> $a \approx 1.96$ 
<!--ID: 1708098043685-->


### Background Info for Confidence Interval
- to find the confidence interval containing $\mu$ with prob $1 - \alpha$, find a such that:
	- #toExplore why it has to be 1-alpha, why dont use the confidence level directly? refer to the normal dis graph for understanding?
	- $P(-a \leq Z \leq a) = 1- \alpha \to P(Z \leq -a) = \frac{\alpha}{2}$
	- $a$ is then labelled $z_\frac{\alpha}{2}$, determined for any $\alpha$ using tech
<!--ID: 1708098043688-->


### Confidence Interval for mean of known std
#### Calculating CI for mean of known std
- For interval containing $\mu$ with prob $1 - \alpha$, sample mean $\bar{x}$
	- sample point estimate - margin of error $\leq$ population point est $\geq$ sample point estimate - margin of error
	- $CI = \bar{x}-z_{\frac{\alpha}{2}}\frac{\sigma}{\sqrt{n}}\leq\mu\leq\bar{x}+z_{\frac{\alpha}{2}}\frac{\sigma}{\sqrt{n}}$
	- sample mean, if unavailable: $=AVERAGE(input, range)$
	- Confidence level of the interval: $(1- \alpha) \cdot 100\%$
	- $(1-\alpha)$: confidence coefficient
	- margin of error: $z_{\frac{\alpha}{2}}\frac{\sigma}{\sqrt{n}}$, 
	- $=CONFIDENCE.NORM(\alpha, \sigma, n)$
	- width of confidence interval: $2 \cdot z_{\frac{\alpha}{2}}\frac{\sigma}{\sqrt{n}}$
	- $\uparrow$ sample size = $\downarrow$ width of interval (CI width is smaller as we have a larger sample size)
	- $\uparrow$  confidence level = $\uparrow$  width of interval
		- [[correlation between confidence level & width of interval]]

#### Determining sample size
- using confidence intervals to estimate population means, $\downarrow$ width of interval = $\uparrow$ sample size 
	- $n=\left({\frac{2\times z_{\frac{\alpha}{2}}\sigma}{w}}\right)^{2}$
	- $\sigma$: population std, $n$: sample size
<!--ID: 1708098043695-->


### Confidence Interval for mean of unknown std 
#### Calculating CI for mean of unknown std
- when $\sigma$ unknown, use same sample to estimate both $\mu$ and $\sigma$ 
- when using sample standard deviation $s$ to estimate $\sigma$, interval estimate for population mean is based on the *t-distribution* 
- Interval estimate of a population mean, $\sigma$ unknown:
	- ${\bar{x}}- t_{\alpha/2}{\frac{s}{\sqrt{n}}} \leq \mu \leq {\bar{x}}+ t_{\alpha/2}{\frac{s}{\sqrt{n}}}$
	- s: sample std
	- Confidence level of the interval: $(1- \alpha) \cdot 100\%$
	- $(1-\alpha)$: confidence coefficient
	- $t_{\alpha / 2}$: find **t-value** from t-distribution with $n-1$ degree of freedom (Excel: T.INV($\frac{1-\alpha}{2}$; df)), take the positive result
	- $n$: sample size, $n \geq 30$ to use this expression
	- margin of error: $t_{\alpha/2}{\frac{s}{\sqrt{n}}}$ CONFIDENCE.T
<!--ID: 1708098043699-->

#### Calculating T-distribution in EXCEL
- calculating t-distribution:  $T.DIST(x, df, cumulative)$: find **probability value** for a given **t-value**
	- `x` : test statistic, or **t-value**
	- `df`: n - 1
	- `cumulative` is a logical value that determines the form of the function. if true, return cdf, else, return pdf
---
<!--ID: 1708098043701-->

### Confidence Interval for Proportion
#### Calculating CI for Proportion
- true population proportion $p$ is unknown -> taking a sample to obtain sample proportion $\bar{p}$ to estimate $p$
- $\bar{p} = X/n$
	- $\bar{p}$: sample proportion
	- $X$: number of successes in the sample
	- n: sample size
- $X \sim B(n,p), EX = np, \sigma_x = \sqrt{np(1-p)}$   
	  -> $E\bar{p} = p$, $\sigma(\bar{p})=\sqrt{\frac{p(1-p)}{n}}$ 
- By [[03. Growth 🌻/probStat/AY2.03. probStat/Central Limit Theorem]], $\bar{p}$ is approximately normally distributed if
	- both $n p\geq5{\mathrm{~and~}}n(1-p)\geq5.$
- **Confidence Interval for p**: 
	- $\bar{p} - z_{\frac{\alpha}{2}}\sqrt{\frac{\bar{p}(1-\bar{p})}{n}} \leq p \leq\ \bar{p} + z_{\frac{\alpha}{2}}\sqrt{\frac{\bar{p}(1-\bar{p})}{n}}$
	- margin of error: $z_{\frac{\alpha}{2}}\sqrt{\frac{\bar{p}(1-\bar{p})}{n}}$
	- width of confidence interval: $2 \cdot z_{\frac{\alpha}{2}}\sqrt{\frac{\bar{p}(1-\bar{p})}{n}}$
<!--ID: 1708098043705-->

#### Determining Sample size
- for $z_{\frac{\alpha}{2}}$ confidence interval, width $w$, preliminary proportion $\bar{p} = p^*$, sample size is
	- $n=\left({\frac{2\times z_{\frac{\alpha}{2}}}{w}}\right)^{2}p^{*}(1-p^{*})$
	- if dont have $\bar{p}$, choose $p^* = 0.5$, as it is worst case, and maximizes $p^*(1-p^*)$ 
---
<!--ID: 1708098043708-->

### Test a claim using confidence interval (a, b)
- [[Test claim using a confidence interval (a, b)]]
<!--ID: 1708098043711-->


### Popular confidence level
| Confidence level | $\alpha$ | $z_{\frac{\alpha}{2}}$ |
| ---- | ---- | ---- |
| 90% | 0.1 | 1.645 |
| 95% | 0.05 | 1.960 |
| 98% | 0.02 | 2.326 |
| 99% | 0.01 | 2.576 |
- find $z_{\frac{\alpha}{2}}$ by using Inverse Normal (casio) with area = $\alpha / 2$ 
<!--ID: 1708098043715-->
