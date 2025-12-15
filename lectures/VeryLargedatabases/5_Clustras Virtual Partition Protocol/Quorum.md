The minimum number of nodes that must agree or respond to perform a read or write operation in a distributed system.
- **n** [[Replication]], every write must be confirmed by **w** nodes
- [[Queries]] at least **r** nodes for each read
- As long as **w + r > n**, we expect to get an up-to-date value
- [[Dynamo-Style]] databases, the parameters **n**, **w** and **r** are typically configurable
- **w = r = (n + 1) / 2** (Rounded up): Common approach
- **w = n** and **r = 1**: Fast reads but all nodes are written
![[Pasted image 20251210231107.png]]
- **W + R < N** may also be valid, giving better response times and less overhead, but you may read stale values
- [[Sloppy Quorums]] may give that read and write [[Quorum]] may be different nodes (no overlap). But increases [[Availability]] for writes
- Concurrent writes may have ordering problems, they may be in conflict. merge conflicts ? [[Last Write Wins (LWW)]] ?
- Concurrent writes and reads may return new or old values
- It should be a pre-defined order of the [[Replication]], primary-backup1-backup2 ... (Not [[Leaderless Replication]])
- Monitoring [[Staleness]] ? Quantify "eventual" [[Consistent]] ?
![[Sloppy Quorums and Hinted Handoff]]
