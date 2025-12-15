- If any of the prepare requests fail or timeout, the coordinator aborts the [[Transactions]]
- If any of the commit or abort requests fail, the coordinator retries them indefinitely
- [[Uncertain or In doubt]]: If the coordinator crashes, the participant can do nothing but wait until the coordinator recovers
![[Pasted image 20251213025804.png]]