The strongest correctness guarantee for [[Concurrency]] [[Transactions]]. It means that even though [[Transactions]] run at the same time, the final result must be the same as if they had run one after another in some serial order.
- [[Isolation Levels]] are hard to understand and inconsistently implemented in different databases
- If you look at your application code, it is difficult to tell whether it is safe to run at a particular [[Isolation Levels]]
- There are no good to help us detect [[Race Conditions]]
- [[Serializable Isolation]] is usually regarded as the strongest [[Isolation Levels]]. It guarantees that even though [[Transactions]] may execute in parallel, the end result is the same as if they had executed one at a time, serially, without any [[Concurrency]]

How do database provide [[Serializability]] ?
- Literally executing [[Transactions]] in a serial order
- [[Two-Phase Locking (2PL)]]
- Optimistic [[Concurrency Control]] techniques
Why run serially ? ([[VoltDB]] / [[H-Store]], [[Redis]], [[Datomic]])
- RAM became cheap enough that for many use cases is now feasible to keep the entire active dataset in memory
- [[Online Transaction Processing (OLTP)]] [[Transactions]] are usually short and only make a small number of reads and writes

- Each [[Transactions]] is through one HTTP request
- Executed by a [[Stored Procedure]]
- No interaction
![[Pasted image 20251212000036.png]]

![[Pros and Cons of Stored Procedures]]

Summary of [[Serial Execution]]:
- Every [[Transactions]] must be small and fast
- The active dataset must fit in memory
- Write throughput must be low enough to be handled on a single CPU core
- [[Cross-Partition Transactions]] are possible, but there is a hard limit to the extent to which they can be used