A clock synchronization algorithm used in [[Distributed System]] to synchronize a client’s clock with a time server, taking network delay into account.

External time server, S ([[Coordinated Universal Time (UTC)]])
- p send messages m_r to S
- S replies with its time t in message m_t
- When p receives m_t, it sets its clock to t + 1/2 of the time passed since m_r was sent
![[Pasted image 20251213042621.png]]