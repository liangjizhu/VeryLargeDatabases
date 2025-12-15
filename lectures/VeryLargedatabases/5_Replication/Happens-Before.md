A partial ordering relation that captures [[Causality]] between events in a [[Distributed System]].
![[Capturing the Happens-Before Relationship]]

![[Pasted image 20251213044454.png]]
- Local events: a -> b; c -> d; e -> f
- Messages: b -> c; d -> f
- Derived: a -> c; a -> f; b -> d
- Concurrent: a || e; b || e; c || e; d || e