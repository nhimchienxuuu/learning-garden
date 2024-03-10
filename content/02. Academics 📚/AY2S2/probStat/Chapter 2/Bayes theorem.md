---
tags:
  - Math/statistic
---
# Bayes theorem:
### Descriptions:
- Can only be used on CDF not PDF
<!--ID: 1708099388672-->

### Proof:
- Let $E$ and $F$ be events, $E=EF\cup EF'$
	- Then $P(E)=P(EF)+P(EF')$ 
	  $=P(E|F).P(F)+P(E|F').P(F')$ 
	  $\color{tomato}\implies P(E)=P(E|F).P(F)+P(E|F').P(F')$
<!--ID: 1708098044011-->

### Special case:
- $\displaystyle P(F|E)=\frac{{\color{tomato}P(F).P(E|F)}}{P(F).P(E|F)+P(F').P(E|F')}= \color{tomato}\frac{P(F\cap E)}{P(E)}$ ^a8c61d
<!--ID: 1708098044016-->


### $\displaystyle P(F_i|E)=\frac{P(F_i).P(E|F_i)}{P(F_1).P(E|F_1)+...+P(F_n).P(E|F_n)}$
- $F_1, F_2,...,F_n$ where all events F are [[Mutually exclusive|mutually exclusive]] events (that is disjoint events) whose [[Union operation|union]] is the sample space where $E$ is an event that has occurred
<!--ID: 1708098044021-->


