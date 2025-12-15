- [[Snapshot Isolation]]: What a read-only [[Transactions]] can see in the presence of [[Concurrent]] writes
- Atomic write (update) operations: (avoid [[Concurrent]] read-write problems)
![[Pasted image 20251211212820.png]]
- Implemented by exclusive lock
- [[Object-Relational Mapping]] [[Framework]] make it easy to accidentally write code that performs unsafe [[Read-Modify-Write Cycle]] instead of using atomic operations provided by the database