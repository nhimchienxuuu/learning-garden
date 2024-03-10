---
tags:
  - Math/statistic
---
# Chebyshev's inequality
### Description:
- If $X$ is a random variable with finite mean $\mu$ and variance $\sigma^2$, then for any value $k > 0,\displaystyle \color{tomato}P(|X - \mu| \ge k) \le \frac{\sigma^2}{k^2}$
- Proof:
	- $\displaystyle P\big((X-\mu)^2\ge k^2\big)\le \frac{E[(X-\mu)^2]}{k^2}$
		- By [[Markov's inequality]]
	- $P\big((X-\mu)^2\ge k^2\big)= P(|X-\mu|\ge k)$
	- Proof complete