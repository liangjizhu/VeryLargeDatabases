- Multiple writes could be rolled back ([[Atomicity]])
- [[Concurrency]] [[Transactions]] may see all writes or none ([[Isolation]])
- SELECT COUNT(\*) FROM emails WHERE recipient_id = 2 AND unread_flag = true
- Slow, so use a cached counter: Anomaly may appear
![[Pasted image 20251211192749.png]]