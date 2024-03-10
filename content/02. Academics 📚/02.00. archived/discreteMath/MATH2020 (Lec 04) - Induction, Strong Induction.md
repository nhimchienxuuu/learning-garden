---

mindmap-plugin: basic

---

# Induction, Strong Induction, Well Ordering Principle

## Induction
- Definition
	- Prove statements are true for any **nonnegative integers** by showing the statement is true for the first integer (base case) and for the next integers (inductive step).
		- Just like recursion.
	- Example: Climb a ladder. Start at the first rung (base case) and show that you can get to the next rung (inductive step) if already on the rung below. Once shown you can get to any rung on the ladder, you can get to all the rungs on the ladder.
- How to Prove
	- **1. Inductive hypothesis**: P(n): statement
	- **2. Base case**: Prove that 1 element is true.
	- **3. Inductive step:** Assume P(n = k) is true, prove that P(k+1) is also true
<!--ID: 1708098041887-->


## A Faulty Induction Proof
### Strong Induction 
- How to Prove
	- **1. Inductive hypothesis**: P(n): statement
	- **2. Base case**: Prove that some base values are true in order to prove for P(n+1)
	- **3. Inductive step:** Assume P(n = k) is true, prove that P(k+1) is also true
- when to use strong induction instead of normal induction
	- solve the inductive step first, whether it is dependent on the previous cases
	- recursion
<!--ID: 1708098041891-->

