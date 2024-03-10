---
mindmap-plugin: basic
create-time: 
tags:
---
# Title
## Context:
- Source: 
- Relation: 
---
## Insight:
- Markov's Inequality
	- X is RV, nonnegative, for any a > 0
	  $P(X\geq\ a)\leq{\frac{E[X]}{a}}$
- Chebyshev's Inequality
	- X is RV, finite mean $\mu$, variance $\sigma^2$, for any k > 0
	  $P(|X-\mu|\geq k)\leq\frac{\sigma^{2}}{k^{2}}$
	- One-side Chebyshev
		- If $E[X] = \mu$ and Var(X) = $\sigma^2$, for a > 0
		  $\begin{array}{c}{{P\{X\geq\mu+a\}\le\frac{\sigma^{2}}{\sigma^{2}\;+\;a^{2}}}}\\ {{P\{X\le\mu\:-\;a\}\le\frac{\sigma^{2}}{\sigma^{2}\,+\;a^{2}}}}\end{array}$
- Purpose of Inequalities above
	- derive bounds on probabilities when mean (and variance) are known
- If $Var(X) = 0$, then $P(X = E[X]) = 1$: the only random variables with variance = 0 are those constant + with probability of 1