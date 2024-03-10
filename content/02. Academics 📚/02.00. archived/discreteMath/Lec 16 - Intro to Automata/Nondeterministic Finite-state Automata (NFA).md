---
tags:
  - Math/discrete/Automata
aliases:
  - NFA
---
# Nondeterministic Finite-state Automata
### Description:
- May have several possible next states for each pair of input value and state
- A Nondeterministic finite-state automata $M=(S,I,f, s_0, F)$:
	- consists of 
		- $S$: a ~~finite~~ set of states
		- $I$: a ~~finite~~ input alphabet
		- $f$: a transition function 
			- assigns a ~~next state~~ **set of states** to each pair of state and input
			- such that $f:S\times I\to \mathcal P(S)$
			- $\mathcal P(S)$ is the power set of S
		- an **starting state**, $s_0$
		- a set of ~~possible accepting~~ **final** states, $F$
			- also a subset of $S$
### NFA's recognized language:
- Let a string $𝑥=𝑥_1 𝑥_2…𝑥_𝑘$ input to an NFA.
- The first input symbol $𝑥_1$ takes the starting state $𝑠_0$ to **a set $𝑆_1$ of states**
- The next input symbol $𝑥_2$ takes **each of the states in $𝑆_1$ to a set of new states**. 
	- Let $𝑆_2$ be the union of these sets.
- Repeat, at each stage, all states obtained using a state obtained at the previous stage and the current input symbol
- The string $𝑥$ is accepted if there is **at least 1 final state in the set of all states** using $𝑥$.
- The language recognized by a NFA is the set of all strings recognized by this NFA.
- #Math/discrete/Automata/theorem
	- If the language $L$ is recognized by a NFA $M_0$, then $L$ is also recognized by a [[Deterministic Finite-state Automata|DFA]] $M_1$
		- where $M_1$ (deterministic) is converted from $M_0$ (Non-deterministic)
		- $M_1$'s states are created from combinations of possible states reached by $M_0$'s states 
			- with **OR** operation
			- combination states where each state can have multiple possible states, the new state of $M_1$ is all of those possible states.
- 1) Q&A - find language recognized by NFA; [question & answer](https://i.imgur.com/8kjWzwK.png)
- 2) Q&A - find a DFA recognized same language as the NFA; [question](https://i.imgur.com/EG0unDi.png), [answer](https://i.imgur.com/kQwcoNT.png)
<!--ID: 1708098041749-->


---
