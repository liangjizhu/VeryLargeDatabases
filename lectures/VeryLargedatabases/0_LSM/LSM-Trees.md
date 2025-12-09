Log-Structured Merge Tree, O'Neil & O'neil 1996
![[Pasted image 20251203022810.png]]
A data structure that optimises for fast writes by using an in-memory structure and multiple on-disk structures using [[key-value store]].

Writes are initially buffered in a fast, in-memory component called a [[Mem-table]]. When it fills up, it is sorted and flushed to disk as a [[Sorted String Table]]. These ones are periodically merged and compacted to improve read performances.

How it works:
- Writes: New data is written to a memory-resident [[Mem-table]]. Because it is a in-memory operation, it is very fast. To ensure data isn't lost during a crash, writes are also appended to a [[Write-Ahead Log (WAL)]]
- Flush: When the [[Mem-table]] is full, its contents are sorted by key and written to disk as a new [[Sorted String Table]].
- Reads: The system first checks the [[Mem-table]]. If not found, it checks the [[Sorted String Table]], starting with the most recent one and backward.
- [[Compaction]]: As more [[Sorted String Table]] are created, compaction merges them. Combines multiple [[Sorted String Table]] into new, larger ones, removes old versions of overwritten data and sorts the data to make reads more efficient.

Advantages:
- Fast writes: high write throughput, as writes are buffered in memory and written to disk in large, sequential batches. [[Sequetial Writes]]
- Write-optimised:  ideal for workloads with high ingest rates, such as event logging or real-time analytics.
- Efficient Merges: [[Compaction]] helps manage disk space and improves read performance by consolidating data.
![[LSM Strength and Weakness]]

![[LSM-Trees_3_Storage_And_Retrieva]]
