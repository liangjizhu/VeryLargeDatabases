A [[Concurrency Control]] technique that makes [[Snapshot Isolation]] behave as if [[Transactions]] were executed serially, without requiring strict locking or blocking.
It provides full [[Serializable Isolation]] while keeping the performance benefits of [[Multi-Version Concurrency Control (MVCC)]].
Used in systems like [[PostgreSQL]] and [[CockRoachDB]]
- [[Two-Phase Locking (2PL)]] is a pessimistic [[Concurrency Control]]
- [[Serializable Snapshot Isolation (SSI)]] is a optimistic [[Concurrency Control]]
- Detecting stale [[Multi-Version Concurrency Control (MVCC)]] reads
![[Pasted image 20251212005503.png]]
- Detecting writes that affect prior reads
![[Pasted image 20251212005528.png]]
Advantages and Performance:
- Compared to [[Two-Phase Locking (2PL)]], the big advantage of [[Serializable Snapshot Isolation (SSI)]] is that one [[Transactions]] doesn't need to block waiting for locks held by another [[Transactions]].
- Compared to [[Serial Execution]], [[Serializable Snapshot Isolation (SSI)]] is not limited to the throughput of a single CPU core
- [[FoundationDB]] distributed the detection of [[Serialization]] conflicts across multiple machines