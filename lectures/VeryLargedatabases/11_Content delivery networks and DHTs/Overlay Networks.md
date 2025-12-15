- You can think of an overlay as a logical network implemented on top of some [[Underlying Network]]
	- By this definition, the Internet started as an [[Overlay Networks]] on top of the links provided by the old telephone network
- Each node in the overlay networks also exists in the underlying network
	- Nodes process and forward packets in an application-specific way
- The links that connect the overlay nodes are implemented as tunnels through the [[Underlying Network]]
![[Pasted image 20251214175100.png]]

- The simplest kind of overlay is one that exists purely to support an alternative routing strategy
	- No additional application-level processing is performed at the nodes
- You can view a [[Virtual Private Network (VPN)]] as an example of a routing overlay
	- In this particular case, the overlay is said to use "IP tunnels"
	- The ability to utilise these [[Virtual Private Network (VPN)]] is supported in many commercial routers

- Suppose, however, you wanted to use a routing algorithm that commercial router vendors were not willing to include in their products
	- You could simply run your algorithm on a collection of end hosts and tunnels through the Internet routers
	- These hosts would behave like routers in the [[Overlay Networks]]
		- As hosts they are probably connected to the Internet by only one physical link, but as a node in the overlay they would be connected to multiple neighbors via tunnels