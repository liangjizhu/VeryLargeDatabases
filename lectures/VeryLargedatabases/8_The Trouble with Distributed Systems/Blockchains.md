A distributed, append-only ledger that stores data in linked blocks, secured by cryptographic hashes, and maintained collectively by a network of nodes without a central authority.
A [[Distributed Ledger System]]
- Shared by all participants
	- Replicated
- Decentralised
- Append-Only
	- No update, no delete
- [[Distributed Transaction Validation]]
	- [[Consensus Systems]]
- [[Unfalsifiable]], verifiable

**Promises**:
- Increased trust in value exchange
	- Trust the data, not the participants
- No single point of failure
	- Increased [[Security]]
- Efficient, [[Consistent]] [[Transactions]] between participants
	- Faster and cheaper than relying on a long of intermediaries, with incompatible systems and rules
![[Public vs Private Blockchain]]

**Concepts**
An immutable [[Distributed Databases]], example: A log of blocks, which are linked and replicated on full nodes
- A block
	- Digital [[Containers]] for [[Transactions]], contracts, property titles, ...
	- [[Transactions]] are secured using public key encryption
	- The code of each new block is built on that of that preceding block
		- Guarantees that it cannot be changed or tampered
- The blockchain is viewed by all participants
	- Privacy: Users are pseudonymised

![[Blockchain Protocol (Nakamoto 2008)]]

Transaction:
- The owner signs the [[Transactions]] by
	- Creating a hash value of
		- The previous [[Transactions]]
		- And the public key (PK) of the next owner
	- Signing it with its secret key (SK)

![[Block Management]]

![[Validation by the Network]]

![[Intentional Fork]]

![[Consensus Protocol]]

![[The 51% Attack]]

![[Transaction Confirmation]]

![[Public Blockchain Limitations]]

![[Blockchain 2]]
