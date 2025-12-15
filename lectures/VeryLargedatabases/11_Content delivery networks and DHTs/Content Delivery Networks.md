![[Web Caching]]

- The idea of a [[Content Distribution Network (CDN)]] is to geographically distribute a collection of server surrogates that cache pages normally maintained in some set of backend servers
	- Thus, rather than have millions of users wait forever to contact, example: www.cnn.com when a big news story breaks - such a situation is known as a [[Flash Crowd]] - it is possible to spread this load across many servers
	- Moreover, rather than having to traverse multiple [[Internet Service Provider (ISP)]]to reach www.cnn.com, if these surrogate servers happen to be spread across all the backbone [[Internet Service Provider (ISP)]], then it should be possible to reach one without having to cross a peering point

![[Applications of CDNs]]

- Proactive content replication
	- Content provider (Example: CNN) contracts with a [[Content Distribution Network (CDN)]]
- [[Content Distribution Network (CDN)]] replicates the content
	- On many servers spread throughout the Internet
- Updating the replicas
	- Updates are pushed to replicas when the content changes
![[Pasted image 20251214140158.png]]
![[Pasted image 20251214140210.png]]
![[Surrogates as Server Replicas]]

![[Types of CDNs]]

![[Relaying CDN]]

![[Partial Replication]]

![[Back-End File System]]

![[Replication Issues]]

![[Request Distribution]]

![[Server Selection Mechanism]]

![[Server Selection Policy]]