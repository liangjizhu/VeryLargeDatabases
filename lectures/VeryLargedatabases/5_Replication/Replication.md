The practice of storing multiple copies of data on different nodes to improve [[Availability]], [[Fault-Tolerant or Resilient]] and read performance.
- Provides [[Redundancy]]
- To keep data geographically close to your users
- [[Fault-Tolerant or Resilient]] - increased [[Availability]]
- Scale out for read queries
- If the data that you are replicating does not change over time, then [[Replication]] is easy
- Replicating changes between nodes:
	- [[Single-Leader]]
	- [[Multi-Leader]]
	- [[Leaderless Replication]]
- [[Synchronous]] vs [[Asynchronous]] [[Replication]]
![[Leader-Based Replication]]
![[Synchronous vs Asynchronous Replication]]
![[Asynchronous Replication]]
![[Adding New Replications (Repair ?)]]
![[Takeover or Failure Handling]]
![[Replication Logs - Statement Based]]
![[Write-Ahead Log-Shipping]]
![[Logical (Row-Based) Log Replication]]
![[Trigger-Based Replication]]
![[Problems with Replication Log]]
![[Reading-Your-Writes Consistency]]

![[Monotonic Reads]]

![[Consistent Prefix Reads]]

![[Solutions for Replication Lag]]

![[Multi-Leader Replication]]

![[Leaderless Replication]]

![[Quorum]]

![[Multi-Datacenter Support]]

![[Detecting Concurrent Writes]]

![[Causality-> Happen Before and Concurrent]]

![[Algorithm to Decide Overwrite or Concurrent]]