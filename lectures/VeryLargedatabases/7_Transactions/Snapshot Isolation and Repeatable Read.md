- Problems with [[Read Committed]]: This anomaly is called a [[Non-Repeatable Read]] or [[Read Skew]] 
![[Pasted image 20251211205219.png]]
- [[Snapshot Isolation]] is the most common solution to this problem. Supported by [[PostgreSQL]], [[MySQL]] / [[InnoDB]], [[Oracle]], [[SQL Server]] and others
- Use write locks, but reads do not require locks
- Readers never block writers, writers never block readers
- [[Multi-Version Concurrency Control (MVCC)]]. Store several versions of an updated record. One for each snapshot
- [[Storage Engine]] that support [[Snapshot Isolation]] typically use [[Multi-Version Concurrency Control (MVCC)]] for their [[Read Committed]] [[Isolation]] level
![[PostgreSQL's MVCC]]

![[Visibility Rules for Observing a Consistent Snapshot]]