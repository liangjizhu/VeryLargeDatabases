- Locking and leader election: All nodes must agree which node owns the lock; otherwise it is useless
- Constraints and [[Uniqueness]] guarantees: A hard [[Uniqueness]] constraint, such as the one you typically find in [[Relational Database]], require [[Linearizability]]
- Cross-Channel timing dependecies:
![[Pasted image 20251213014154.png]]