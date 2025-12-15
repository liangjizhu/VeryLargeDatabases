The component or API through which users or applications formulate and submit queries to retrieve or manipulate data in a system.
Methods:
- get(t, k) -> v
	- Returns all attributes of the row in table t that has the key k
- put(t, k, v)
	- Inserts a new row in table t that has key k and value v
- verify() -> bool
	- For put(t, k, v), it means whether or not the put was actually committed in the [[Storage Layer]]
	- For a get(t, k) it is checked whether or not the returned value was correct or a spurious value