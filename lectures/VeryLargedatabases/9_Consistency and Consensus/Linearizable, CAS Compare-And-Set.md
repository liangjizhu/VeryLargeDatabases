- cas(x, v_old, v_new) -> r means the client requested an atomic [[Compare-And-Set]] on variable x
- An atomic [[Compare-And-Set]] (cas) operation can be used to check the value hasn't been concurrently changed by another client
- The requirement of [[Linearizability]] is that the lines joining up the operation markers always move forward in time (from left to right), never backward
![[Pasted image 20251212234740.png]]