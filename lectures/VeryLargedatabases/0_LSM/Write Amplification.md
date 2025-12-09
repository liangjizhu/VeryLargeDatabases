When a [[SSDs]] writes a larger amount of data to its flash memory than the host system requested, which negatively impacts performance and longevity. This happens because [[SSDs]] write data in small pages but can only erase data in large blocks, so updating even a small amount of data requires erasing and rewriting an entire block. This process is exacerbated by internal operations like [[Garbage Collection]] and [[Wear Leveling]].
- #bytes written to datases / #bytes written to [[API]] 
- [[B-Trees]]: Less [[Write Amplification]] with big records
- [[LSM-Trees]]: Less [[Write Amplification]] due to big write chunks, but [[Compaction]] require more writes
- [[LSM-Trees]]: [[Write Amplification]] independent on record size
- May be measured by insert throughput. [[RocksDB]] performs very well.
