- Allow more than one node to accept writes
- [[Multi-Leader]], master/slave or active/active replication
- A leader in each datacenter
![[Pasted image 20251210223834.png]]
- Performance (Local writes)
- Tolerance of datacenter outages
- Tolerance of network problems
- May cause [[Concurrency]] update to the same data: Thus, needs conflict resolution
- Disconnected databases, example calendar, have the same problem
- Collaborative editing (Google docs, Office365)
![[Handling Write Conflicts]]

![[Conflict Resolution]]

![[Multi-Leader Replication Topologies]]