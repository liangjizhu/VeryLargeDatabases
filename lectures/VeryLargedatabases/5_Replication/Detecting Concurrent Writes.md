- Problem: Events may arrive in a different order at different nodes, due to a variable network delays and partial failures.
![[Pasted image 20251210233833.png]]
Solutions:
- [[Last Write Wins (LWW)]]
- Some way of unambiguously determining which write is more "recent"
- We can attach a timestamp to each write, pick the biggest timestamp as the most "recent" and discard any writes with an earlier timestamp