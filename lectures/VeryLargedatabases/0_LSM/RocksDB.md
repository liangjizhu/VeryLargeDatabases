- Builds on Google's [[LevelDB]] and [[Apache HBase]]
- [[Multi-threaded Compaction]]
- Multi-threaded insertion into [[Mem-table]]
- Extensive control over [[Bloom filters]]
- Multicore and [[SSDs]] support
- 10x improved write performance compared to [[LevelDB]] due to [[Multi-threaded Compaction]]
![[Pasted image 20251203024743.png]]
- [[SST File]] (sorted key ranges)
- [[Mem-table]]
- [[Write-Ahead Log (WAL)]]
![[Leveled Compaction]]
![[LSM Strength and Weakness]]
![[Universal Compaction]]
![[Bloom filters]]