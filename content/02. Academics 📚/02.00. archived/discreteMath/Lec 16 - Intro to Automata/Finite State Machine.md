---
tags:
  - Math/discrete/Automata
aliases:
  - Finite Automata
  - FA
  - Finite-state Automata
---
# Finite State Machine
### Description:
- Mathematical model of computation  
- Can be in exactly one of a finite number of states at any given time.
- A finite-state automata $M=(S,I,f, s_0, F)$:
	- consists of 
		- $S$: a finite set of states
		- $I$: a finite input alphabet
		- $f$: a transition function 
			- assigns a next state to every pair of state and input
			- such that $f:S\times I\to S$
		- an initial or final state, $s_0$
		- a set of possible accepting state, $F$
			- also a subset of $S$
	- [example question](https://i.imgur.com/LVKeuGd.png) and my [attempt solution](https://i.imgur.com/0yLzj4n.png)
### Types of FA
- FA without output:
	- [[Deterministic Finite-state Automata]]
	- [[Nondeterministic Finite-state Automata (NFA)]]
- FA with output:
	- [[Moore Machine]]
	- [[Mealy Machine]]
<!--ID: 1708098041728-->

### Transition:
- To change FA from one state to another in response to some inputs
<!--ID: 1708098041732-->

### Accept/reject string:
- A [[Automata Theory#String|string]] is said to be **recognized** or **accepted** by the machine, $M=(S,I,f, s_0, F)$, if it takes the initial state $s_0$ to a final state, that is $f(s_0,x)$, is a state in $F$. 
- example:
	- [sample state machine](https://i.imgur.com/pAdl2lD.png)
	- *(question)* 𝑥=01011, what is $𝑓(𝑠_0,𝑥)$? Is it accepted? 
		- *(answer)* Yes
		- $𝑓(𝑠_0,𝑥)$ = ==S0== S1 S1 S0 ==S1==, take from the initial to final state
	- *(question)* 𝑦=00110, what is $𝑓(𝑠_0,𝑦)$? Is it accepted?
		- *(answer)* No
		- $𝑓(𝑠_0,𝑥)$ = ==S0== S0 S1 S0 ==S0==, doesnt take from init to final state
<!--ID: 1708098041736-->

### Language recognition by FSM
- The **language** recognized or accepted by the machine $M$, denoted by $\color{skyblue}L(M)$, is the set of all strings that are accepted by $M$
- Determine languages recognized by a machine M:
	- define final state(s) of M
	- per each final state, determine the string that take the initial to its final state
- [example](https://i.imgur.com/mryRTuw.png)
<!--ID: 1708098041739-->

### Equivalent finite-state automata:
- Definition: Two finite-state automata are called equivalent if they recognize the same language
	- Meaning accept the same set of inputs
- [example question & solution](https://i.imgur.com/CGT1ntu.png)
<!--ID: 1708098041741-->


### State table:
- ![](https://media.geeksforgeeks.org/wp-content/uploads/20210828221222/capture2.png)
<!--ID: 1708098041743-->
