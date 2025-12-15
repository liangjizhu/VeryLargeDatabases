A mechanism for tracking [[Causality]] and detecting [[Concurrency]] events in [[Distributed System]].

- [[Logical Clocks (Lamport)]] only get you so far
- To figure out more about event order, we need to store / transfer more info
- [[Vector Clocks]], given N processes
	- Every process has a vector of N elements
	- Contains the number of events from each process that the given process can have been affected by
Definitions:
- V_i - Vector at process i
- Initially all vector elements = 0
- Before each events at p_i:
	- V_i[i] = V_i[i] + 1
- p_i attaches t = V_i to all messages
- When p_i receives a message
	- V_i[j] = max(V_i[j], t[j]), for j = 1, 2, ..., N
	- (Also V_i[i] = V_i[i] + 1)
![[Pasted image 20251213045830.png]]
- If e -> e' then V(e) < V(e')              As before
- If V(e) < V(e') then e -> e'
	- V < V' iff V <= V' and V not equal V'
	- <= and = must hold for all pairs of vector elements