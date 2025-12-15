- The biggest problem with [[Multi-Leader Replication]]
![[Pasted image 20251210224043.png]]
- [[Synchronous]] vs [[Asynchronous]] conflict detection
- [[Conflict Avoidance]]: Allow updates only at one site for each data item
- Converging to a [[Consistent]] state:
	- There is no "correct" values when you have write conflicts, however, [[Consistent]] values are the goal:
		- Each write has a unique ID (example: timestamp),  [[Last Write Wins (LWW)]]
		- Each [[Replication]] has a unique ID, and higher ID "wins"
		- Merge values and keep all of them (B and C in the example)
		- Apply [[Conflict Resolution]] on them (Automatic or manual)
