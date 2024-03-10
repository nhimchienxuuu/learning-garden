---
mindmap-plugin: basic
tags:
  - Math/statistic/theorem
---
# The DeMoivre-Laplace limit theorem
### Description:
- Special case of [[03. Growth 🌻/probStat/Chapter 10/Central limit theorem]] of de Moivre-Laplace
- If $S_n$ denotes the number of success that occur when $n$ independent trials, each resulting in a success with probability $p$ ([[Binomial distribution]]), are performed, then, for any $a<b$, $$P\bigg(a\le \frac{S_{p}-np}{\sqrt{np(1-p)}}\le b\bigg)\to \Phi (b)-\Phi(a)$$
	- as $n\to \infty$, where:$$\Phi(x)=\frac{1}{\sqrt {2\pi}}\int^{x}_{-\infty}e^{-y^2/2}dy$$
