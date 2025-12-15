![[Pasted image 20251213024449.png]]
- Coordinator
- Participants
- If all participants reply "yes", indicating they are ready to commit, then the coordinator sends out a commit request in phase 2
- If any of the participants replies "no", the coordinator sends an abort request to all nodes in phase 2
- [[Commitment]]:
	- It's like bacon and eggs
	- The chicken participates
	- The pig is committed
- Request a [[Transactions]] ID from the coordinator
- Start execution on all nodes. Any node may decide to abort
- When [[Ready-To-Commit]], the coordinator sends a [[Prepare-To-Commit]] to all participants
- Participants receive [[Prepare-To-Commit]] and replies yes or no
- Coordinator receives all and decides. [[Log]]s the decision
- The commit or abort message is sent to all participants
- Done is returned from all participants
![[Coordinator Failure]]

Performance:
- Too costly ?: Due to the addition [[Disk Forcing (fsync)]] that is required for crash recovery and the additional network [[Round-Trip Time (RTT)]]
- Two types of [[Distributed Transactions]]
	- Databases-Internal [[Distributed Transactions]]
	- Heterogeneous [[Distributed Transactions]]
- [[XA Protocol]]: a C [[API]] for interfacing with a [[Transactions]] coordinator. Standard [[Two-Phase Commit (2PC)]] support
- The coordinator is usually a library that is loaded into the same process as the application issuing the [[Transactions]]

![[Holding Locks While In Doubt]]

![[Limitations of Distributed Transactions (XA)]]