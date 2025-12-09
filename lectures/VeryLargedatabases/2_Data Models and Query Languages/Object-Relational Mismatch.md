- Mismatch between application code and database model (objects vs rows)
- [[Object-Relational Mapping]] ([[SQLAlchemy]], [[Prisma]], [[ActiveRecord]] and [[Hibernate]]) try to hide the difference
- Example:
	- [[LinkedIn]] resume (3 solutions in [[SQL]]):
		- [[Normalised]]: position, education and contact information, using foreign keys
		- [[Structured Datatypes]] / [[XML]] / [[JSON]] inside rows. Querying and indexing these
		- [[JSON]] / [[XML]] documents inside text columns containing Position, Education and Contact Information. Let application [[query]] and decode
	- Tables and Foreign Keys
		![[Pasted image 20251207170742.png]]
	- ![[JSON]]