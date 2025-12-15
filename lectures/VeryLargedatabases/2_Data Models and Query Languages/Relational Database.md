Organises data into structured tables (relations) with rows (records) and columns (attributes) that are linked by common data points (keys) to show clear relationships, making data easy to manage, query and analyse, unlike flat files, with popular examples being [[MySQL]], [[Oracle]] and [[SQL Server]].

- [[ER Modeling]]
- [[Relational Schema]]
- Organise data in tables
	- ![[Pasted image 20251214202617.png]]
- Use indexes to speed-up access

Pro:
- Flexible by design
- Familiar [[Boyce–Codd Normal Form (BCNF)]] (strong mathematical backgroud)
- [[Transactions]] and [[ACID - Properties of a Transaction]]
- Very "mature" and well tested (mostly)
- Easy adoption / integration
Cons:
- Large and unstructured data
- Lots of random I/Os are often [[Write-Heavy]] 
- **Not built for distributed applications / environments**
- **Single point of failure**
- Speed ([[Performance]]), example: Not fast enough for specialised applications
- **[[Scaling Up (Vertical Scaling)]], not out**:
	- [[Scaling Up (Vertical Scaling)]]: Grow capacity by replacing old machines with newer ones
	- [[Scaling Out (Horizontal Scaling)]]: Incrementally grow capacity by adding more [[Commercial Off-The-Shelf (COTS)]]
![[Pasted image 20251214203220.png]]