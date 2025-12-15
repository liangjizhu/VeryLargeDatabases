[[MapReduce]]
- Google created (2003) it to support internet crawl:
	SELECT map() FROM crawl_table GROUP BY reduce()
- map() and reduce() written in a programming language
- Yahoo created [[Apache Hadoop]] (2005)
- [[Google File System (GFS)]] and [[Hadoop Distributed File System (HDFS)]] file systems
- Many enterprises spent a lot of money on [[Apache Hadoop]] clusters, only to find there was little interest in this functionality
- Google announced that they were moving their crawl processing from [[MapReduce]] to [[BigTable]]. The reason was that Google needed to interactively update its [[Crawl Databases]] in real-time but [[MapReduce]] was a batch system (2014)
- There was considerable efforts to provide a [[SQL]] and [[MapReduce]] interface on top of [[Apache Hadoop]], most notable was Meta's [[Apache Hive]], later replaced by [[Facebook Presto]]: [[SQL]] on everything
- [[Facebook Presto]]: Connector [[API]] allows plugins to provide an I/O interface to dozens of data sources, including [[Apache Hadoop]] [[Data Warehousing (DW)]], [[Relational Database Management System (RDBMS)]], [[NoSQL]] systems and [[Stream Processing]] systems
- [[Apache Hadoop]] died about a decade ago, [[Apache Spark]] and [[Apache Flink]] are new implementations with support for [[SQL]]