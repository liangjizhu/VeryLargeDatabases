Locks that protect a range of index values rather than individual rows. They are used by databases to prevent phantom reads and ensure serializable or repeatable-read behaviour.
- Also called [[Next-Key Locking]]
- Simplified approximation of [[Predicate Locks]]
- Lock index entries to the data set you are searching
- Shared locks
- Example: room_id or start_time / end_time in the room booking