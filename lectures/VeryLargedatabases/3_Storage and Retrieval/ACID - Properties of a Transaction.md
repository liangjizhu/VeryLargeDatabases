[[Atomicity]], [[Consistency]], [[Isolation]] and [[Durability]]
[[Transactions]]: A sequence of operations on DB which are:
- **A** - Atomic: Completely run or not
- **C** - Consistency: (primary key, references, check, ...)
- **I** - Isolation: Does not notice other [[Transactions]]
- **D** - Durability: Nothing lost after commit
A [[Transactions]] is usually a logical operation or task
[[Kleppmann]]: The high-level idea is sound, but the devil is in the details. Today, when a system claims to be "[[ACID - Properties of a Transaction]] compliant", it is unclear what guarantees you can actually expect. [[ACID - Properties of a Transaction]] has unfortunately become mostly a marketing term.
- [[BASE]] is "not [[ACID - Properties of a Transaction]]"
![[Atomicity]]
![[Consistency]]
![[Isolation]]
![[Durability]]

![[Single-Object and Multi-Object Operations]]

