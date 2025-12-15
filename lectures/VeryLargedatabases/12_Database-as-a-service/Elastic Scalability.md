Workload exceeds single machine capacity
- Scale a single database to multiple nodes
- [[Scaling Out (Horizontal Scaling)]] by [[Queries]] processing [[Partitioning]]
- Granular placement and load balancing on backend
Strategy well suited for [[Online Transaction Processing (OLTP)]] and Web workloads... but can extend to [[Online Analytical Processing (OLAP)]]
Minimise cross-node [[Distributed Transactions]]
[[Workload-Aware Partitioner]]
- [[Partitions]] data to minimise multi-node [[Transactions]]
- Front-end analyses execution traces represented as a graph
	- Each tuple is a node and two nodes are connected when accessed together in a [[Transactions]]