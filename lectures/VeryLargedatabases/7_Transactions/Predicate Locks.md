A type of lock used in database [[Concurrency Control]] that locks all rows that satisfy a logical condition (a predicate)—including rows that currently exist and rows that might exist in the future.
- Locking a search condition, so that you can have a [[Consistent]] read
![[Pasted image 20251212003016.png]]
- Transaction A must acquire a shared-mode [[Predicate Locks]] on the conditions of the [[Queries]]
- If transaction B currently has an exclusive lock matching those conditions, A must wait until B releases its lock
- Predicate locks apply even to objects that do not yet exist