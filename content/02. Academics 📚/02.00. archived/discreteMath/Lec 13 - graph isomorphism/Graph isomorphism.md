---
tags:
  - Math/discrete/graph
aliases:
  - Isomorphic
---
# Graph isomorphism
### Description:
- Graph $G_1$ and $G_2$ are isomorphism if there exists a bijection $f: V_1 \to V_2$ such that $(u,v)\in E_1$ if and only if $(f(u),f(v))\in E_2$.
	- The bijection $f$ is called the isomorphism from $G_1$ to $G_2$
	- Notation: $G_2=f(G_1)$
- There are $n!$ possible bijections
- Graph invariant (property preserved by isomorphism of graphs):
	- Have same number of edges and vertices
	- Same degree of vertices
	- Same cycle structure
### Interactive proof:
- Prove that two graph are not isomorphic
- Proof:
	- Consider, a prover $P$ and a verifier $V$
	- Input: $G_0=(V=\{1,...,n\}, E_0)$ and $G_1=(V=\{1,...,n\}, E_1)$ allegedly not isomorphic
	- Step 1: $V$ picks a random permutation/bijection 𝜋: {1, ... , 𝑛} → {1, ... , 𝑛}, a random bit 𝑏 ∈ {0,1}, and send $H=\pi (G_b)$ to $P$
	- Step 2: $P$ checks if $H$ is isomorphic to $G_0$ or $G_1$ (in polynomial time) and send $b'=0$ or $b'=1$ to $V$, respectively
	- Step 3: $V$ accepts (that the graph are non-isomorphic) is and only if $b'=b$
- Completeness: ?
	- If the graphs are not isomorphic, then 𝐻 is isomorphic to 𝐺! , but not to the other input graph 𝐺"#! . This allows P to determine 𝑏′ = 𝑏 every time
- Soundness:
	- If the graphs are isomorphic, then 𝐻 is isomorphic to both 𝐺$ and 𝐺" . Therefore, it is impossible to tell from which input graph is used by V. With probability 1/2, we have 𝑏≠ 𝑏 and the verifier rejects
<!--ID: 1708098041651-->



