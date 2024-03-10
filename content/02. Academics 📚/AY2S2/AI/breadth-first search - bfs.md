---
time: 
tags: 
child:
---
## note
- Strategy: expand a shallowest node first
- Implementation: fringe is a FIFO queue
- Properties:
	- Time complexity: $O(b^s)$
		- s tiers -> there will be s nodes of b in the worst case time
	- Space complexity: $O(b^s)$
	- Complete: yes
	- Optimal: only if costs are all 1
- ![](https://i.imgur.com/FIK2NSv.png)
