![[Evolvability]]
![[Formats For Encoding Data]]
![[Data Formatting Languages (Textual)]]
![[Binary Encoding]]
![[MessagePack]]
![[Thrift and Protocol Buffers]]
![[Thrift's BinaryProtocol]]
![[Thrift's CompactProtocol]]
![[Protocol Buffers]]
![[Schema Evolution]]
![[Apache Avro]]
![[Reader's and Writer's Schema]]
![[Advantages of Using Schema]]
![[Dataflow through Databases]]
![[Dataflow through Services REST or RPC]]
![[Web Services]]![[Problems with RPCs]]
![[The Future for RPC]]

![[Message Passing Dataflow]]

![[Distributed Actor Frameworks]]

Summary:
- Data encoding should support [[Rolling Upgrades]] 
- Must ensure [[Backward Compatibility]]
- Programming language solutions - Efficient, but locked
- Textual formats like [[JSON]], [[XML]] and [[CSV]] support [[Schemas]], but are vague about datatypes
- Binary [[Schemas]] - Driven formats like [[Apache Thrift]], [[Protocol Buffers]] and [[Apache Avro]] allow compact, efficient encoding
- Modes of dataflow
	- Through databases
	- [[RPC]] and [[RESTful HTTP API]]
	- [[Message-Passing]]
