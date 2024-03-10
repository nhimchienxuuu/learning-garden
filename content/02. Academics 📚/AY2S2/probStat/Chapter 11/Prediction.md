---
tags:
  - Math/statistic
---
# Prediction
### Description:
- A random variable $X$ is observed, and then an attempt is made to predict the value of a random variable $Y$ .  
- Let $g (X )$ denote the predictor
	- that is, if $X$ is observed to equal $x$
	- then $g (x)$ is our prediction for the value of $Y$ . 
	- We want to choose $g$ so that $g (X )$ tends to be close to $Y$ .  
- One possible way is to choose $g$ to minimize $E[(Y-g(X))^2]$
	- The best possible preditor is $g(X)=E(Y|X)$
- Proposition:
	- $E[(Y-g(X))^2]\ge E[(Y-E[Y|X])^2]$
	- $Var(X)=0$ then $P(X=E[X])=1$
---