A [[NoSQL]] database that uses nodes (entities) and edges (relationships) to store data as a connected network, focusing on the relationships between data points rather than rigid [[Tables]], making it ideal for complex, interconnected data like [[Social Networks]], [[Fraud Detection]] or [[Recommendation Engines]].
- Many applications use [[Knowledge Graph]] to model [[Semi-Structured]] information
- Social media application inherently contrain [[Graph-Oriented Relationship]] ("likes", "friend-of")
- (1) [[Resource Description Framework (RDF)]] [[Triple-Stores]]
- (2) [[Property Graphs]]
- Operational / [[Online Transaction Processing (OLTP)]] workload: [[Neo4j]]. Follow [[Chain of Links]]
- [[Analytics]]: Derive information from the graph. Example: finding which user has the most friends under 30 yo: [[TigerGraph]] and [[JanusGraph]]
- Distribution is difficult: Compress a graph into a space-efficient data structure that fits in memory on a single node and then run the [[Queries]] against this data structure
- [[SQL]]: 2023 introduced [[Property Graph Queries (PGQ)]] ([[SQL]] / [[Property Graph Queries (PGQ)]])