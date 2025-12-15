A type of [[NoSQL]] database that stores data in document-like structures (usually [[JSON]] or [[BSON]]), rather than rows and columns. Each document is a self-contained, semi-structured object that can have nested fields and varying [[Schemas]].
- Each document contains a hierarchy of [[Field-Value Pairs]], where each field is identified by a name and a field's value can be either a scalar type, an array of values or another document
- {"name": "First Last", "orders":[
	{"id": 123, "items": [...]},
	{"id":456, "items": [...]},
	] }
- [[Database Management Systems (DBMS)]] that stored records or documents as [[JSON]], supported a lower-level [[API]] and weak or non-existent [[Transactions]]. Example: [[MongoDB]]
- Removes the [[Impedance]] mismatch between how application Object-Oriented code interacts with data
- ![[Denormalisation]]
- Adding [[SQL]] and [[ACID - Properties of a Transaction]] to a [[NoSQL]] [[Database Management Systems (DBMS)]] lowers their intellectual distance from [[Relational Database Management System (RDBMS)]]
- Higher level languages are almost universally preferred to record-at-a-time notations as they require less code and provide greater data independence
- But the optimiser remains the hardest part of building a [[Database Management Systems (DBMS)]]
- We suspect that this [[Engineering Burden]] was a contributing factor to thy [[NoSQL]] systems originally chose to not support [[SQL]]