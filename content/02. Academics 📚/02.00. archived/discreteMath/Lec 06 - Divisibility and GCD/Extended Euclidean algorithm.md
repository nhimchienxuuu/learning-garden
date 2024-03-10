---
mindmap-plugin: basic
tags:
  - Math/discrete/theorem
aliases:
  - Be ́zout’s theorem
---

# Extended Euclidean algorithm

## Description:
- Sub title
	- Let $a, b ∈ N^+$, $a, b$ not both 0. Then, there exist $s, t ∈ Z$ such that $sa + tb = gcd(a, b)$ #Math/discrete/theorem
- Extended Euclidean algorithm
	- Find two integers $a$ and $b$ such that $1914a+899b=gcd⁡(1914,899)$
	- First use Euclid's algorithm to find the GCD:
		- $1914=2×899+116$
		- $899=7×116+87$
		- $116=1×87+29$
		- $87=3×29+0$
	- From this, the last non-zero remainder (GCD) is $29$.
	- Now we use the extended algorithm:
		- $29=116+(−1)×87$
		- $87=899+(−7)×116$​
	- Substituting for 8787 in the first equation, we have
	- $29=116+(−1)×(899+(−7)×116)$
	- $=(−1)×899+8×116$
	- $=(−1)×899+8×(1914+(−2)×899)$
	- $=8×1914+(−17)×899$​

## Implementation:

-
  ```python
  def extended_gcd(a, b):
  if b == 0:
  return (a, 1, 0)
  else: s, t, d = extended_gcd(b, a % b)
  return (d, t, s - a // b * t)
  ```
<!--ID: 1708098041358-->
