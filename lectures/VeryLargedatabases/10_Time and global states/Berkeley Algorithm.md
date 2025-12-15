A clock synchronization algorithm for [[Distributed System]] where a master node periodically synchronizes the clocks of all other nodes, without relying on an external time source.

One node selected as master
- The master polls all other nodes (slaves)
- Slaves reply with their local time
- Master calculates average time
	- Message latency considered
	- Ignored outliers
- Master sends individual differences to each slave (why differences ?)