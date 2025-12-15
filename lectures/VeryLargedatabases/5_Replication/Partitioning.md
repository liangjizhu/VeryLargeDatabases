The process of dividing data into smaller subsets (partitions) and distributing them across multiple nodes ([[Sharding or Partitioning]]) to improve [[scalability]] and performance.
- For very large datasets, or very high [[Queries]] throughput
- We need to break the data up into [[Partitions]]
	- Shards ([[MongoDB]], [[ElasticSearch]])
	- Region ([[Apache HBase]])
	- Vnode ([[Apache Cassandra]], [[Riak]])
	- vBucket ([[Couchbase]])
- [[Scalability]] is the main reason for [[Partitioning]]
- [[Load Sharing]] is another reason
![[Query Execution and Partitioning]]
![[Partitioning and Replication]]
![[Range Partitioning]]
![[Hash Partitioning]]![[Skewed Workloads and Hot Spots]]
![[Document-Based Indexing]]

![[Term-Based Indexing]]

![[Rebalancing Partitions]]

![[Dynamic Partitioning (Range Partitioning)]]

![[Request Routing]]

![[Coordination of Services]]

Summary:
- [[Hash Partitioning]]
- Key [[Range Partitioning]]
- [[Document-Based Indexing]] ([[Local Indexing]])
- [[Term-Based Indexing]] ([[Global Indexing]])
- [[Rebalancing Partitions]]
- [[Request Routing]]
- [[Coordination of Services]]