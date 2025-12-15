- Also as active/passive, master/slave and primary/backup, primary/hot-standby
- Writes sent to leader which writes the changes to disk
- Followers (read replicas, slaves, secondaries or hot standbys) are sent the changes through a [[Replication]] [[Streams (Multiple Calls and Replies)]] / [[Change Log]]
- Must apply all writes in the same order as they were processed on the leader
- Any [[Replication]] may be read, but only master accepts writes
- [[PostgreSQL]], [[MySQL]], [[Oracle Data Guard]] and [[SQL Server]]'s [[AlwaysOn Availability Groups]], [[MongoDB]], ...
![[Pasted image 20251210012633.png]]