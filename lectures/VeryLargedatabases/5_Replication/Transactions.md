A mechanism for grouping multiple operations into one logical unit of work with well-defined correctness guarantees.
They are necessary because:
- The database software or hardware may fail at any time
- The application may crash at any time
- Interruptions in the network cause apps to be lost from database
- Several clients may have [[Concurrency]], conflicting writes
- A client may read data that doesn't make sense due to partial updates
- [[Race Conditions]] between clients can cause surprising bugs
- The user wants to abort the [[Transactions]]

- Used to group several reads and writes together into a logical unit
- Commits or aborts as an unit
- May be retried in case of abort
- Used to simplify the programming model for applications accessing a database
- Some applications don't need (user-level) [[Transactions]]
- Concepts to learn: Read committed, snapshot isolation and [[Serializability]]

![[History of Transactions]]

![[ACID - Properties of a Transaction]]

![[Transactions and Atomicity]]

![[Single Object Writes]]
![[The Need for Multi-Object Transactions]]

![[Handling Errors and Aborts]]

![[Weak Isolation Levels]]

![[Read Committed]]

![[MVCC, Indexes and COW-B+-Trees]]

![[Repeatable Read and the SQL "Standard"]]

![[Preventing Lost Updates]]

![[Explicit Locking]]

![[Compare-And-Set]]

![[Conflict Resolution and Replication]]

![[Write Skew and Phantoms]]

![[Serializability]]

![[Two-Phase Locking (2PL)]]

![[Predicate Locks]]

![[Index-Range Locks]]

![[Serializable Snapshot Isolation (SSI)]]