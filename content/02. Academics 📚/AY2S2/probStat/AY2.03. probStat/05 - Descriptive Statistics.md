---

mindmap-plugin: basic

---

# Descriptive Statistics

## frequency distributions
- records number of times each value occur
<!--ID: 1708098043506-->


## arithmetic mean
- sum of values of items / number of items
<!--ID: 1708098043511-->

## the mode
- Definition: value that appears most often in a set of data
- In a grouped frequency distribution
	- define the modal class (class with largest frequency)
	- use the formula: 
			  $$
		\begin{equation}
		\text{Mode} = L + \frac{{d_1}}{{d_1 + d_2}} \cdot h
		\end{equation}
			  $$
		$L$: the lower boundary of the modal class 
		$d1​ (d2​)$: absolute value of the difference between the frequency of the class modal and the class before (after) it 
		$h$: length of the interval of the modal class.
<!--ID: 1708098043514-->


## the median
- Definition: the number in the middle of a sorted data set.
	- even-size data set: average of 2 middle numbers
	- odd-size data set: middle number
<!--ID: 1708098043520-->


## Range:
- the difference between the largest and the smallest value
<!--ID: 1708098043522-->

## Percentile:
- a measure indicates value BELOW which a given percentage of observations in a group of observations falls
	- eg. 20th percentile = value below which 20% of observations found
- Find location of the `Pth` percentile $Lp = (n+1)\cdot\frac{P}{100}$
	$L$: location in the ordered array of the desired percentile
	$n$: number of observations
	$P$: desired percentile
- Find percentile based on location:$Pth = value\;at\;lower\;Lp + P\cdot value\;(higher\;-\;lower)\;Lp$
<!--ID: 1708098043525-->

## Quartiles
- Definition: three points divide dataset into 4 equal groups, each comprises a quarter of the data
- $Q_1 = P_{25},\;Q_2 = P_{50},\;Q_3 = P_{75}$
	$Q_1$ : middle number btw smallest & median
	$Q2$: median
	$Q3$: middle value btw median & highest
<!--ID: 1708098043529-->


## Deciles
- any of nine values divide sorted data into 10 equal parts, each represents 10% of the sample / population
- just like Percentile, for eg `8th Decile = 80% Percentile`
<!--ID: 1708098043531-->


## Percentile with grouped data
- calculate from frequency table
	$loc$: from  $P_n$ calculate the location -> determine the class from the cumulative frequency (round up)
	$P_{n} = first\; class\; value + (last\;cum\;freq\;to\;this\;loc) \cdot\frac{{class\;range}}{{frequency}}$
<!--ID: 1708098043534-->

## Inter-quartile range (IQR)
- $$IQR = Q_3 - Q_1 = P_{75} - P_{25}$$
<!--ID: 1708098043539-->

## Variance
- the average of the squared mean deviation for each value in a distribution
- normal variance
	- $$\sigma^2 = \frac{\sum_{i=1}^{n} (x_i - \bar{x})^2}{n}
	$$
		$x_i$: individual observation
		$\bar{x}$ : population mean
		$n$: number of observations
- Variance with grouped data
	- $$\sigma^2 = \frac{\sum fM^2 - n\bar{x}^2}{n}
	$$
		$f$: class frequency
		$M$: class midpoint
		$n$: number of observations
<!--ID: 1708098043543-->

## Standard deviation: 
- square root of the variance $$\sigma = \sqrt{\sigma^2}
$$
- Standard deviation: in finance, can measure the risk associated with various investment opportunities. the higher the std, the greater the risk
- Two investments with similar std may have different distribution of returns
<!--ID: 1708098043547-->


## symmetry
- one that can be divided into two mirrored halves of each other, with same arithmetic mean, median, and mode ("bell curve")
<!--ID: 1708098043549-->

## skewness
- the asymmetry of a frequency distribution curve, with different mean, mode, median
	- positive skewed distribution: lean left (just like holding left thumb), $mean > median$
	- negative skewed distribution: lean right (just like holding right thumb), $mean < median$
<!--ID: 1708098043553-->


## hard parts -> cheat sheet
- interpretation of the Quartiles
<!--ID: 1708098043557-->
