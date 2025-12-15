- Many computers send packets to the same destination, the [[Network Switch]] must queue them up and feed them into the destination network link one by one
![[Pasted image 20251212025341.png]]
- If all CPU cores are currently busy, the incoming request from the network is queued by the operating system until the application is ready to handle it
- In virtulized environments, a running operating system is often paused for tens of milliseconds
- [[TCP or IP]] / [[UDP]] may add delays at sender node (to wait for more data, or to limit sending data)
- [[Timeout]]: Systems can continually measure response times and automatically adjust timeouts according to the observed response time distribution