- The data in each peer is stored in a [[Tamper-Proof Log]] 
	- Any data modification of the log by any potentially malicious party could be detected since the cryptographic hashes used in the [[Blockchains]] would not be valid anymore
- All parties read only from their local copy of the database
	- [[Spurious Reads]] (that are a problem if data needs to be read from a remote party) can be avoided
- Problem: [[Performance]]
Main idea
- Implement a database layer on top of an existing [[Blockchains]]
- Simple-To-Use abstraction with a put / get
- Stores all data in its storage layer that relies on [[Blockchains]]
Goals
- Provide all the benefits of the [[Blockchains]] along with high performance
How does [[BlockchainDB]] achieve these goals:
- [[Partitioning]] and [[Partial Replication]]
- [[Queries]] interface and [[Consistency]]



