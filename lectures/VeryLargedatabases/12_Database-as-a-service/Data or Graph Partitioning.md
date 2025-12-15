![[Pasted image 20251215000100.png]]
![[Pasted image 20251215000113.png]]
![[Pasted image 20251215000126.png]]
![[Pasted image 20251215000139.png]]
![[Pasted image 20251215000149.png]]
![[Pasted image 20251215000200.png]]
![[Pasted image 20251215000214.png]]
![[Pasted image 20251215000224.png]]
![[Graph Partitioning]]
Data Partitioning
- The output of the partitioner is an assignment of individual tuples to logical partitions
- The naive approach leads to a graph with N nodes and up to N^2 edges for an N-tuple database
- Heuristics to reduce the size of the graph
	- Blanket statement removal, example: The exclusion form the graph of occasional statements that scan large portions of the database
	- Sampling tuples and [[Transactions]]