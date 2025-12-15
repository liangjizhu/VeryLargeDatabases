A structured [[P2P Networks]] overlay network and a well-known implementation of a [[Distributed Hash Table (DHT)]]
- Given a key, [[Chord]] maps the key to a node
- Each node should maintain information for a few nodes
	- [[Chord]] achieves O(logN)
- Balance the load by distributing roughly evenly keys to nodes
- Involve little movement of keys when nodes join or leave the system
	- [[Chord]] achieves O(log2N)

![[Chord - Base Protocol]]

![[Chord - Lookup]]

![[Chord - Node Insertion]]

![[Chord - Node Deletion]]

![[Benefits of Chord]]