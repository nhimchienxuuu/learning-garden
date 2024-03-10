---
tags:
  - Math/discrete/Automata
aliases:
  - DFA
---
# Deterministic Finite-state Automata
### Description:
- Simple model, limited memory, has exactly 1 state at any given time
- each pair of state and input value mapped to a unique next state
	- deterministic, opposite to [[Nondeterministic Finite-state Automata (NFA)]]
	- unlike eg, dice
- Can only transition to 1 more state
- example
	- two states $s_0$ and $s_1$
	- $s_0$ is the start state, $s_1$ is the final state
	- input alphabet is $I = \{0,1\}$
	- *next state* is depending on the *current state* and *the input*
- ![|200](https://i.imgur.com/1dXzuzK.png)

