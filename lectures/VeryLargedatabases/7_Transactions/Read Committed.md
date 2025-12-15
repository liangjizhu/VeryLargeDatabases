- When reading from the database, you will only see data that has been committed (no [[Dirty Reads]])
- When writing to the database, you will only overwrite data that has been committed (no [[Dirty Writes]])
![[Pasted image 20251211204247.png]]
- If a [[Transactions]] needs to update several objects, a [[Dirty Reads]] means that another transaction may see some of the updates but not others
- If the database allows [[Dirty Reads]], that means a [[Transactions]] may see data that is later rolled back
![[No Dirty Writes]]
- [[Read Committed]] is a very popular [[Isolation Levels]]. It is the default setting in [[Oracle]] 11g, [[PostgreSQL]], [[SQL Server]] 2012, [[MemSQL]], ...
- Most databases prevent [[Dirty Reads]] by keeping old values for writes until the [[Transactions]] commit. Read [[Transactions]] may read the old value
- Only when the new value is committed do [[Transactions]] switch over to reading the new value
- To keep single record locks would cost too much, since one writer may cause multiple readers to wait

![[Snapshot Isolation and Repeatable Read]]