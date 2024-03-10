---
tags:
  - Math/statistic
---
# Confidence interval
### Description:
- From a **Sample**
- Based on [[Distribution of sample mean]]
### For mean of known standard deviation:
- A confidence interval for a **Population mean** $\mu$, is an interval of values between two limits, together with a percentage indicating our confidence that $\mu$ lies in that interval
	- For $\displaystyle Z=\frac{\bar X_n-\mu}{\sigma/\sqrt n}$
		- By [[03. Growth 🌻/probStat/Chapter 10/Central limit theorem]]
	- $\displaystyle P(-a\le Z\le a)=\alpha\to P(Z\le a)=1-\frac{\alpha}2 +\alpha= z_{\frac{\alpha}2}$
		- $\alpha$ is the **area under graph** between 2 limits while $z_{\alpha/2}$ is the upper limit
	- $\displaystyle CI = \bigg\{\bar x_n - {\color{tomato} z_{\frac \alpha 2 }}\frac{\sigma}{\sqrt n} \le \mu \le \bar x_n + {\color{tomato}z_{\frac \alpha 2}}\frac{\sigma}{\sqrt n}\bigg\}$
- The width is then $2\times z_{\frac \alpha 2 }\frac{\sigma}{\sqrt n}$ 

### For mean of unknown sd:
- Use [[t distribution]]

### For population proportional:
- True population proportion $p$ is unknown
- $\displaystyle \bar p= \frac X n$ 
	- where $X$ is [[Binomial distribution|binomial random variable]] denotes the number of successes in the sample
	- $X\sim B(n,p). E[X]=np$ and $\sigma_X=\sqrt{npq}$
- $E[\bar p]=p$ and $\sigma(\bar p)=\sqrt{\frac{pq}{n}}$
- By [[03. Growth 🌻/probStat/Chapter 10/Central limit theorem]], $\displaystyle \bar p\sim N(p,\frac{pq}{n})$
	- For $np>5$ and $nq>5$
- $\displaystyle\ \alpha \text{CI}=\bar p\pm z_{\alpha/2}\sqrt{\frac{\bar p (1-\bar p)}{n}}$

### For difference of two variables:
- [[Difference random variable of 2 variables]]
- For known $\sigma$
	- $\displaystyle CI(\alpha)=\bar x_1-\bar x_2\pm z_{\alpha/2}\sqrt{\frac{\sigma^2_1}{n_1}+\frac{\sigma^2_2}{n_2}}$
- For unknown $\sigma$
	- $\displaystyle CI(\alpha)=\bar x_1-\bar x_2\pm t_{\alpha/2}\sqrt{\frac{s^2_1}{n_1}+\frac{s^2_2}{n_2}}$

$\\( x = {-b \pm \sqrt{b^2-4ac} \over 2a} \\)$

