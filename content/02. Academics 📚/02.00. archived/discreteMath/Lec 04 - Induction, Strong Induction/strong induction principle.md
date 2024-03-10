---
mindmap-plugin: basic
tags:
  - Math/discrete/principle
---
# Strong induction
### Description:
- Allows us to make a stronger assumption in the inductive step. 
- Mathematical induction proves that we can climb as high as we like on a ladder, by proving that
	- we can climb on the bottom rung (base case) 
	- we can climb ==all== the previous rung then we can climb the next one
### Strong induction principle:
- How to Prove
	- **1. Inductive hypothesis**: P(n): statement
	- **2. Base case**: Prove that some base values are true in order to prove for P(n+1)
	- **3. Inductive step:** Assume P(n = k) is true, prove that P(k+1) is also true
- when to use strong induction instead of normal induction
	- solve the inductive step first, whether it is dependent on the previous cases
	- recursion
<!--ID: 1708098041155-->

