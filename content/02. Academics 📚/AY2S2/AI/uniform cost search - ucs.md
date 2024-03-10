---
time: 
tags: 
child:
---
## what is uniform cost search
- Strategy: expand a cheapest node first
- Implementation: fringe is a priority queue (priority: cumulative cost)
- Properties: (if the solution cost C* and arc costs at least 𝜺 -> effective depth is roughly C*/𝜺
	- Time complexity: $\\(O(b^{C*/𝜺})\\)$
	- Space complexity: $\\(O(b^{C*/𝜺})\\)$
	- Complete: yes (if C* and 𝜺 are finite and positive)
	- Optimal: yes
- [pic](https://i.imgur.com/ZcFchuF.png)
- Good? 
	- complete & optimal
- Bad?
	- explore options in every direction
	- no info about goal location