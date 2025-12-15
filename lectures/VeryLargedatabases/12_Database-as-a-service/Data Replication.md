- A relation or fragment of a relation is replicated if it is stored redundantly in two or more sites
- Full replication of a relation is the case where the relation is stored at all sites
- Fully redundant databases are those in which every site contains a copy of the entire database
Advantages:
- [[Availability]]
	- If replicas exist, failure of the site containing relation r does not result in the unavailability of r
- [[Parallelism]]
	- [[Queries]] on r may be processed by several nodes in parallel
- [[Reduced Data Transfer]]
	- The relation r is available locally at each site, containing a replica of r
Disadvantages:
- Increased cost of updates
	- Each replica of relation r must be updated
- Increased complexity of [[Concurrency Control]]
	- Concurrent updates to distinct replicas may lead to inconsistent data unless special [[Concurrency Control]] mechanisms are implemented
	- One solution
		- Choose one copy as the primary copy and apply [[Concurrency Control]] operations on the primary copy