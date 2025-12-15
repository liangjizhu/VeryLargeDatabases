The technique of storing copies of web resources (e.g. [[HTML]] pages, images, [[API]] responses) so future requests can be served faster and without contacting the original server.
![[Pasted image 20251214134148.png]]
- Cache "close" to the client
	- Under the administrative control of the client-side
- [[Explicit Proxy]]
	- Requires configuring the browser
- [[Implicit Proxy (Transparent Proxy)]]
	- Service provider deploys an "on path" proxy that intercepts and handles Web requests

- Cache "close" to the server
	- Either by [[Proxy]] run by the server or in a third-party [[Content Distribution Network (CDN)]]
- Directing clients to the [[Proxy]]
	- Map the site name to the IP address of the [[Proxy]]

- ![[Proxy Caches]]
- ![[Limitations of Web Caching]]