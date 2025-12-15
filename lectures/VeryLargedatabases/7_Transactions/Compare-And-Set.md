[[Compare-And-Swap]]
An atomic primitive used in [[Concurrent]] and [[Distributed System]] to safely perform [[Read-Modify-Write Cycle]] operations without locks.
- Used by some databases without [[Transactions]], often called [[LightWeight Transactions (LWT)]] 
- The purpose of this operation is to avoid lost updates by allowing an update to happen only if the value has not changed since you last read it
![[Pasted image 20251211231741.png]]
- If the content has changed and no longer matches "old content", this update will have no effect, so you need to check whether the update took effect and retry

![[Linearizable, CAS Compare-And-Set]]