---
tags:
  - Math/statistic
---
# Conditional variance
### Description:
- [[Conditional joint distribution]]'s [[Variance]]
- Conditional variance of $X$ given that $Y = y$ 
	- $Var(X|Y ) = E[(X −E[X|Y ])2|Y] = E[X^2|Y ] − (E[X|Y ])^2$
	- Hence $E[Var(X|Y)] = E[E[X^2|Y ]] − E[(E[X|Y ])^2] = E[X^2] − E[(E[X|Y ])^2]$
	- Also, since $E[E[X|Y ]] = E[X]$, we have $Var(E[X|Y ]) = E[(E[X|Y ])^2] − (E[X])^2$
	- Adding the last two equations, we have $Var(X)=E[{\color{tomato}Var(X|Y)]+Var(E[X|Y]})$
	- 