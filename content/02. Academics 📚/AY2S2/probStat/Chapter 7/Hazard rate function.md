---
mindmap-plugin: basic
tags:
  - Math/statistic
aliases:
  - failure rate function
---

# Hazard rate (failure rate) function

## Description:
- Describe the probability of an item's failure happen $t$, given that the item is still functioning ^5e2a9f
- Consider a positive continuous random variable $X$ be the lifetime (existing without failure) of some item.
- Let $X$ have distribution function $F$ (probability of it failing before $t$) and density $f$. ^77d67f
- The hazard rate function $λ(t)$ of $F$ is defined by $λ(t) = \frac{f(t)}{\bar F(t)}=\frac{f(t)}{1- F(t)}$ ^5687e6
	- where $\bar F=1-F$ , probability of it will fail after time $t$
	- Conditional probability of (it failing in the next $dt$ time) given (not yet fail after $t$-unit old)
- The parameter λ is often referred to as the ==rate== of the distribution.
- $F(t)$, probability of lifetime less than $t$, is: $$\color {tomato}F(t)=1-\exp\bigg({-\int^{t}_{0}\lambda(t)dt\bigg)}$$ ^3cd644