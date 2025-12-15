A fundamental correctness property ensuring that an operation is executed completely or not at all.
- Atomic refers to something that cannot be broken down into smaller parts
- In [[ACID - Properties of a Transaction]], [[Atomicity]] is not about [[Concurrency]]
- [[ACID - Properties of a Transaction]] [[Atomicity]] describes what happens if a client wants to make several writes (and reads)
- [[Atomicity]] simplifies the problem of half-done operations:
	- If a [[Transactions]] was aborted, the application can be sure that it didn't change anything, so it can safely be retried
- [[Kleppmann]]: [[Abortability]] is a better word