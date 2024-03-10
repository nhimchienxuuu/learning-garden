---

mindmap-plugin: basic

---

# Discrete Random Variables

## discrete random var definition
- random var taking at most a countable number of values -> discrete -> DRV
<!--ID: 1708098043639-->


## probability mass function
- for a DRV X, p(a) of X: $p(a) = P(X=a)$
	- positive for at most a countable number of values of a
	$p(x_i) \geq 0\;for\;i = 1,2,...$
	$\sum_{i=1}^{\infty}p(x_i) = 1$
<!--ID: 1708098043644-->


## Expected Value / Expectation: average outcome of a RV
- if x is DRV with $p(x)$ -> expectation / expected value of X, $E[X]$:
$$E[X] = \sum_{x:p(x)>0}^{}xp(x)$$
- a game with $E[X]$ = 0 is a fair game
	- each player has equal chance of winning or losing
	- probability of winning = probability of losing
	- eg. flip coins, Casino games are NOT a fair game
<!--ID: 1708098043647-->


## Proposition
- if X is DRV taking on 1 of values $x_i, i \geq 1$, with respective probabilities $p(x_i)$, then, for any real-valued function $g$ ^484c8dbb-1a4c-10ce
	- $$E[g(x)] = \sum_{i}^{}g(x_i)p(x_i)$$
<!--ID: 1708099388699-->


## Corollary
- if a and b are const
$$E[aX + b] = aE[X] + b$$
<!--ID: 1708099388700-->


## Variance
- if X is RV with mean $\mu$ , then Var(X) is the expectation of the square of difference between X and its mean
$$Var(X) = E[(X - \mu)^2] = E[X^2] - (E[X])^2
$$
<!--ID: 1708099388701-->


## Standard Deviation
- $$
\sigma(X) = \sqrt{Var(X)}
$$
- Proof
$$
Var(X) = E[X^2] - (E[X])^2
$$
$$
Var(aX+b) = a^2Var(X)
$$
<!--ID: 1708098043655-->


## Bernoulli Random Variables
- Suppose a trial whose outcome is either success or failure. If letting X = 1 when success, X = 0 when failure, the probability mass function of X is:
$p(0) = P(X=0) = 1-p$
$p(1) = P(X = 1) = p$
with $p, 0 \leq p \leq 1$ is the probability of success trial
-> random variable X is Bernoulli Random Variable (BerRV)
-> a BerRV is just BinoRV with parameter $(1,p)$
<!--ID: 1708098043658-->


## Binomial Random Variable
- $n$ independent trials, each results in success with probability $p$, or failure with probability $1-p$. Denote $X$ as successes occur in the $n$ trials -> $X$ is binomial random variable with parameter $(n,p)$
<!--ID: 1708098043662-->


## Binomial Experiment
- same experiment repeated in fixed number of times
- only 2 outcomes, success or failure
- repeated trials are independent, so that probability of success remans same for each trial
<!--ID: 1708098043666-->


## Binomial Probability
- If p is probability of success in single trial of a bino experiment, the prob of x successes and n-x failures, in n independent repeated trials of the experiment, known as bino probability
	- $P(x \text{ successes in } n \text{ trials}) = \binom{n}{x}p^x(1-p)^{n-x}$
- If X is bino RV with para n and p
	- $E[X] = np$
	- $Var(X) = np(1-p)$
<!--ID: 1708098043669-->


## Poisson Random Variable
- a RV X taking on one of the values 0,1,2,... is a PRV with para $\lambda$ if, for some $\lambda > 0, i = 0,1,2,\ldots$
	- $p(i) = P(X = i) = e^{-\lambda} \frac{\lambda^i}{i!}, \quad i = 0,1,2,\ldots$
	- $\lambda$ is average rate of value
- This equation defines a probability mass function, since
	- $\sum_{i=0}^{\infty} p(i) = e^{-\lambda} \cdot \sum_{i=0}^{\infty} \frac{\lambda^i}{i!} = e^{-\lambda}\cdot e^{\lambda} = 1$
- PRV can be used as approx for BinoRV
$X \sim B(n,p)$: $n$ is large, $p$ is small, $\lambda = np$ moderate size
$X \sim Po(\lambda) -> P(X=i) = e^{-\lambda} \frac{\lambda^i}{i!}$
- For $n$ large and $\lambda$ moderate
$$(1 - \frac{\lambda}{n})^n \approx e^{-\lambda}$$
$$\frac{n(n - 1)...(n - i + 1)}{n^i} \approx 1$$
$$(1 - \frac{\lambda}{n})^i \approx 1$$
Then $$P(X = i) \approx e^{-\lambda} \cdot \frac{\lambda^i}{i!}$$
- Expected Value & Variance
$$E[X] = Var(X) = E[X^2] - (E[X])^2 = \lambda $$
$$E[X^2] = \lambda\cdot(1-\lambda)$$
- Computing the Poisson Distribution Function
	- If $X$ is Poisson with parameter $\lambda$, then
	$$\frac{P(X = i + 1)}{P(X = i)}= \frac{\lambda}{i+1}$$
	- Starting with $P(X=0) = e^{-\lambda}$, we can use:
	$P(X = 1) = \lambda P(X = 0)$
	$P(X = 2) = \frac{\lambda}{2} P(X = 1)$
	$\vdots$
	$P(X = i + 1) = \frac{\lambda}{i + 1} P(X = i)$
<!--ID: 1708098043672-->


## Cumulative Distribution Function
- For a random variable X
$F(x) = P(X \leq x), \quad -\infty < x < \infty$
is called the cumulative distribution function of X
	- 1. F is a non-decreasing function
	- 2. $\lim_{x \to \infty} F(x) = 1$
	- 3. $\lim_{x \to -\infty} F(x) = 0$
	- 4. F is right continuous. That is, for any $b$ and any decreasing sequence $b_n, n \geq 1,$ that converges to b, $\lim_{n \to \infty} F(b_n) = F(b)$
- $P(X \leq k) = e^{-\lambda} \cdot \sum_{i=0}^{k} \frac{\lambda^i}{i!}$
<!--ID: 1708098043677-->
