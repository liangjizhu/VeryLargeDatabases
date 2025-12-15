Single-Node case: Two clients adding items to the same shopping cart
![[Pasted image 20251210234529.png]]
- The database returns multiple values (siblings), which the client may merge in
![[Pasted image 20251210234617.png]]
- The database doesn't need to check values, just look at version numbers
- Must use [[Tombstones]] for deletes
- [[Version Vectors]] (Multiple replicas) and [[Vector Clocks]] (Multiple Nodes): Must use multiple version / state numbers