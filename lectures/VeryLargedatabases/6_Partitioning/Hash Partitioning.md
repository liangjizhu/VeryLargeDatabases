A data [[Partitioning]] strategy where each data item is assigned to a partition by applying a hash function to its key.
![[Pasted image 20251211172502.png]]
- A good hash function takes skewed data and makes it uniformly distributed
	- [[Apache Cassandra]] and [[MongoDB]] use [[MD5]]
	- [[Voldemort]] uses the [[Fowler-Noll-Vo (FNV) Hash Function]]
- Gives good load balance, but no range scans. You have to do range scans on all partitions ([[MongoDB]])
	- [[Apache Cassandra]] may use [[Compound Keys]], where only the first part is hashed
	![[Pasted image 20251211173036.png]]