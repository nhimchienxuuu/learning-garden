---
mindmap-plugin: basic
tags:
  - Math/statistic
---
# Conditional Probability:
### $P(A|B)=\frac{P(A\cap B)}{P(B)}$
- $P(A\cap B)=P(B).P(A|B)=P(A).P(B|A)$:  ^328612
	- Probability of the [[Intersect operation|intersection]] of 2 events
- $P(A_1, A_2,A_3,...,A_n)=P(A_1)\ . \ P(A_2|A_1)\ . \ P(A_3| A_1, A_2)\ ...\ P(A_n, A_1, A_2,...,A_n)$:
	- Probability of the [[Intersect operation|intersection]] of n events - chain rule
<!--ID: 1708098044033-->

### Independence:
- Event A and B are independent if any of the 3 conditions hold: ^6a4bf6
	1. $P(A|B)=A$
	2. $P(B|A)=B$
	3. $P(A\cap B)=P(A).P(B)$: product rule for independent event
		- Use this to find independence: $P(A\cap B)=P(A)+P(B)-P(A\cap B)$
- Events A, B and C are independent if all following equations hold: ^a3a924
	1. $P(A, B)=P(A)P(B)$
	2. $P(B, C)=P(B)P(C)$
	3. $P(C, A)=P(C)P(A)$
	4. $P(A, B, C)=P(A)P(B)P(C)$
<!--ID: 1708098044036-->

### Conditional independence: $P(A\cap B)=P(A|B)P(B)$
- Event A and B are conditional independent given an event C:
	- $P(A,B|C)=P(A|C)P(B|C)$
- [[Bayes theorem]]
<!--ID: 1708098044040-->



