A weak [[Consistent]] model where [[Replication]] may temporarily diverge, but will converge to the same state over time if no new updates occur.
- Ensures that if no new updates are made to a given data item, eventually all read accesses to that item will return the last value
- Implementation in [[BlockchainDB]]
	- Execute each incoming read operation of a client immedaitely
- [[Staleness]]
	- [[Pending-Write Queue]] might grow quickly
	- [[BlockchainDB]] might return stale values
- Solution: Set a bound on the size of the [[Pending-Write Queue]]
	- This limit is user-defined and provides a trade-off between [[Staleness]] and [[Latency]]