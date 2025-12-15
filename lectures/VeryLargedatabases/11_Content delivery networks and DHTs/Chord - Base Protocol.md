- Keys are ordered binary numbers of length m
- Nodes are also assigned an ID in the same number space
- Nodes are ordered in a ring according to their IDs
- For a given key k is the responsible node n is the one with the smallest id larger than k, also called successor(k)
![[Pasted image 20251214191832.png]]
- Each node p maintains a finger table with a most m entries
					FT_p[i] = succ(p + 2^(i-1))
- To look up a key k, node p forwards the request to node with index j satisfying
					q = FT_p[j] <= k < FT_p[j + 1]
- If p < k < FT_p[1], the request is also forwarded to FT_p[1]