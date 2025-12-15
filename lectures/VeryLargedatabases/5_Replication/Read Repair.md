A technique used in eventually [[Consistent]], [[Dynamo-Style]] systems to fix [[Replication]] inconsistencies during read operations.
- A read request is sent to multiple replicas.
- The system compares returned versions.
- If some replicas have stale data, the newest/correct version is written back to them.