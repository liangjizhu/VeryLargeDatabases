One of the ACID properties, guaranteeing that once a transaction commits, its effects persist permanently, even in the presence of crashes or failures.
- Is the promise that once a transaction has committed successfully, any data it has written will not be forgotten
- Usually done by [[Write-Ahead Log (WAL)]] ([[Force-Log-At-Commit]]). Some oldtype databases forces data to disk
- Force / Steal classification ([[Theo Harder]])
- Force data or force redo log (example: no-force)
- Steal slot in buffer (force undo log) or no-steal