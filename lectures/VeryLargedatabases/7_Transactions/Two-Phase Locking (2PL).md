A classic [[Concurrency Control]] protocol that guarantees conflict [[Serializability]] by enforcing a specific rule on how [[Transactions]] acquire and release locks.
- Several [[Transactions]] are allowed to concurrently read the same object as long as nobody is writing to it
- If [[Transactions]] A has read an object and [[Transactions]] B wants to write to that object, B must wait until A commits or aborts before it can continue
- If [[Transactions]] A has written an object and [[Transactions]] B wants to read that object, B must wait until A commits or aborts before it can continue
- [[Two-Phase Locking (2PL)]] is used by the [[Serializable Isolation]] level in [[MySQL]] ([[InnoDB]]) and [[SQL Server]], and the [[Repeatable Read]] [[Isolation Levels]] in [[DB2]]

- T wants to read an object: T must acquire the lock in shared mode. Several [[Transactions]] are allowed to hold the lock in shared mode simultaneously
- T wants to write to an object: T must first acquire the lock in exclusive mode. No other [[Transactions]] may hold the lock at the same time
- T first reads and then writes an object, it may upgrade its shared lock to an exclusive lock
- After a [[Transactions]] has acquired the lock, it must continue to hold the lock until the end of the [[Transactions]] (commit or abort)

![[Performance of Two-Phase Locking (2PL)]]