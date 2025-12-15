A mechanism that requires a participant to perform computational work before a request or transaction is accepted, making abuse costly.
- Computed by each miner to produce the [[Nonce]]
- Goal: Produce a value v such that h(f(block, v)) < T where
	- h is the SHA-256 hash function
	- T is a target value shared by all nodes that reflects the network size
	- f is a function that combines v with information in the block
	- v is a 256-bit number starting with n zero bits