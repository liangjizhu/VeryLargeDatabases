![[Transactions]]

Summary:
- [[Transactions]] are abstractions to simplify error handling
- [[Isolation Levels]]: [[Read Committed]], [[Snapshot Isolation]] ([[Repeatable Read]]) and serializable
- Problems:
	- [[Dirty Reads]]
	- [[Dirty Writes]]
	- [[Read Skew]] ([[Non-Repeatable Read]])
	- Lost Updates
	- [[Write Skew]]
	- [[Phantom Read]]
- Solutions to serializable
	- [[Serial Execution]]
	- [[Two-Phase Locking (2PL)]]
	- [[Serializable Snapshot Isolation (SSI)]]