The abstraction and set of operations through which higher layers of a system interact with the storage layer.
Main methods:
- read(s, k) -> v
	- Reads a value v for a given shard s and a key k
- write-async(s, k, v) -> tx-id
	- Write a value v with key k into shard s
- check-tx-status(s, tx-id) -> TX-STATUS
	- Check the status of a write-async operation, example: COMMITED, ABORTED, PENDING
- get-writeset(s, e) -> ws
	- Returns all writes that were executed on shard s in epoch e